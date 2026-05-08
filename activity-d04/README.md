# CLCT 4000: Activity D04 - File & Share Permissions

## Setup Environment & Virtualization

**Host Operating System:** macOS (Apple Silicon / Mac)
**Target Environment:** Windows 11 ARM64 (Virtual Machine via UTM)

---

## Activity 1: Configuring and Managing Local and Share Permissions

**Scenario:** Create file shares for Marketing and IT departments in `C:\Data`. Ensure strict access control where only IT members can access the IT share.

### Step-by-Step Implementation:

#### Step 1: Create Groups
1. Open **Computer Management** > **Local Users and Groups** > **Groups**.
2. Right-click and select **New Group**.
3. Create `MarketingGroup` and `ITGroup`.

![Step 1: Local Groups Created](./images/local_groups_creation.png)

#### Step 2: Create Folders
1. Open File Explorer and navigate to `C:\`.
2. Create a folder named **Data**.
3. Inside **Data**, create subfolders named **Marketing** and **IT**.

![Step 2: Folders Created](./images/folders_creation.png)

#### Step 3: Configure NTFS (Security) Permissions
1. Right-click the **IT** folder > **Properties** > **Security**.
2. Click **Advanced** > **Disable inheritance** > **Remove all inherited permissions from this object**.
3. Click **Add** > **Select a principal** > Type `ITGroup`.
4. Grant **Full Control** to the **ITGroup**.
5. Repeat similar steps for the **Marketing** folder and **MarketingGroup**.

![Step 3: NTFS Permissions Set](./images/ntfs_security_settings.png)

#### Step 4: Configure Share Permissions
1. Right-click the **IT** folder > **Properties** > **Sharing** > **Advanced Sharing**.
2. Check **Share this folder**.
3. Click **Permissions**.
4. Remove "Everyone" and add **ITGroup** with **Full Control** (or Change).
5. Repeat for the **Marketing** folder.

![Step 4: Share Permissions Set](./images/share_permissions_settings.png)

#### Step 5: Verification
1. Log in as a user who is *not* in the ITGroup and try to access the IT folder.
2. Verify that access is denied.

![Step 5: Access Denied Verification](./images/access_denied_verification.png)

---
*End of Activity D04 Document*

