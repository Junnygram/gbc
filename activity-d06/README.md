# CLCT 4000: Activity D06 - App Management & System Updates

## Setup Environment & Virtualization

**Host Operating System:** macOS (Apple Silicon / Mac)
**Target Environment:** Windows 11 ARM64 (Virtual Machine via UTM)

---

## Activity 1: Microsoft Store App Management

**Scenario:** Install, update, and uninstall Microsoft OneNote via the Store.

### Step-by-Step Implementation:
1. Open the **Microsoft Store** app.
2. Search for **OneNote** and click **Install**.

![OneNote Installation](./images/onenote_install.png)

3. Go to **Library** (bottom left) and click **Get updates** to demonstrate updating apps.

![Store Library Updates](./images/store_updates.png)

4. Go to Start, right-click **OneNote**, and select **Uninstall** to demonstrate the full lifecycle.

![App Uninstallation](./images/app_uninstall.png)

---

## Activity 2: Windows Package Manager (winget)

**Scenario:** Use `winget` to search for and install **PowerToys**.

### Step-by-Step Implementation:
1. Open **Command Prompt** or **PowerShell**.
2. Type `winget search PowerToys` and press Enter.
3. Type `winget install Microsoft.PowerToys`.

![Winget Installation](./images/winget_powertoys.png)

---

## Activity 3: Microsoft Edge Synchronization

**Scenario:** Configure synchronization settings between two virtual devices.

### Step-by-Step Implementation:
1. Open **Microsoft Edge**.
2. Sign in with your Microsoft account.
3. Go to **Settings** > **Profiles** > **Sync**.
4. Verify that **Favorites**, **Settings**, and **Extensions** are set to Sync.

![Edge Sync Settings](./images/edge_sync.png)

---

## Activity 4: Configuring Windows Update

**Scenario:** Configure advanced update settings and pause updates.

### Step-by-Step Implementation:
1. Go to **Settings** > **Windows Update** > **Advanced options**.
2. Enable **"Receive updates for other Microsoft products"**.
3. Set **Active hours** to Manual (7:00 AM to 8:00 PM).

![Update Advanced Options](./images/update_advanced_options.png)

4. On the main Windows Update page, click **Pause for 1 week** (or 2 weeks).

![Updates Paused](./images/updates_paused.png)

---
*End of Activity D06 Document*

