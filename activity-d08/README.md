# CLCT 4000: Activity D08 - Maintenance & Recovery

## Setup Environment & Virtualization

**Host Operating System:** macOS (Apple Silicon / Mac)
**Target Environment:** Windows 11 ARM64 (Virtual Machine via UTM)

---

## Activity 1: Windows Event Logs

**Scenario:** Identify system errors and configure log sizes and archival policies.

### Step-by-Step Implementation:
1. Open **Event Viewer**.
2. Go to **Windows Logs** > **System**.
3. Click **Filter Current Log...** and check **Warning** and **Error**.

![Filtered Event Logs](./images/filtered_event_logs.png)

4. **Log Size:** Right-click **Application** log > **Properties**. Set the maximum size to **20480 KB**.

![Application Log Properties](./images/app_log_size.png)

5. **Archiving:** For the **Security** log, select **"Archive the log when full, do not overwrite events"**.

![Security Log Archiving](./images/security_log_archiving.png)

---

## Activity 2: Performance Monitoring

**Scenario:** Use Task Manager and Reliability Monitor to identify issues.

### Step-by-Step Implementation:
1. Open **Task Manager** > **Performance** tab to monitor CPU and Memory usage.

![Task Manager Performance](./images/task_manager_performance.png)

2. Search for and open **Reliability Monitor**. Review the stability chart.

![Reliability Monitor](./images/reliability_monitor.png)

---

## Activity 3: Registry Editor Customization

**Scenario:** Change the Registered Owner and Organization.

### Step-by-Step Implementation:
1. Open `regedit` and navigate to: `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion`.
2. Change **RegisteredOwner** to "Administrator" and **RegisteredOrganization** to "Contoso Corp".

![Registry Editor Change](./images/registry_edit_owner.png)

3. Run `winver` to verify the changes.

![Winver Verification](./images/winver_verification.png)

---

## Activity 4 & 5: File History & Custom Folders

**Scenario:** Use File History to protect custom folders.

### Step-by-Step Implementation:
1. Go to **Control Panel** > **File History**.
2. Click **Select drive** and choose your backup location (Network or Drive).

![File History Setup](./images/file_history_setup.png)

3. Add the **Data** and **Reports** folders to your **Documents Library**.
4. Verify they are now being protected by File History.

![Library Inclusion](./images/library_inclusion.png)

---

## Activity 6: Recovering Windows (Reset This PC)

**Scenario:** Reset the PC while keeping user files.

### Step-by-Step Implementation:
1. Go to **Settings** > **System** > **Recovery** > **Reset PC**.
2. Select **Keep my files**.

![Reset This PC Screen](./images/reset_pc_keep_files.png)

---
*End of Activity D08 Document*

