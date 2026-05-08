# CLCT 4000: Activity D07 - Security, Firewall & BitLocker

## Setup Environment & Virtualization

**Host Operating System:** macOS (Apple Silicon / Mac)
**Target Environment:** Windows 11 ARM64 (Virtual Machine via UTM)

---

## Activity 1: Microsoft Defender & Threat Detection

**Scenario:** Configure protection settings and simulate a virus using a test file.

### Step-by-Step Implementation:

#### Step 1: Controlled Folder Access
1. Go to **Windows Security** > **Virus & threat protection** > **Manage ransomware protection**.
2. Toggle **Controlled folder access** to **On**.

![Controlled Folder Access](./images/controlled_folder_access.png)

#### Step 2: Virus Simulation
1. Create a folder `C:\Files`.
2. Create a file `sample.txt` inside it.
3. Paste the EICAR test string into the file and save.
4. Verify that Microsoft Defender flags the threat.

![Threat Detection Proof](./images/defender_threat_detection.png)

#### Step 3: Exclusions
1. In Defender settings, go to **Exclusions** > **Add or remove exclusions**.
2. Add the `C:\Files` folder.
3. Re-create the test file and verify it is no longer flagged.

![Defender Exclusions](./images/defender_exclusions.png)

---

## Activity 2: Windows Security Settings

**Scenario:** Verify SmartScreen and Exploit Protection status.

### Step-by-Step Implementation:
1. Go to **Windows Security** > **App & browser control** > **Reputation-based protection settings**.
2. Verify **SmartScreen** is enabled.

![SmartScreen Status](./images/smartscreen_status.png)

---

## Activity 3: Inbound Firewall Rules

**Scenario:** Block Remote Desktop connections via Firewall.

### Step-by-Step Implementation:
1. Open **Windows Defender Firewall with Advanced Security**.
2. Go to **Inbound Rules** > **New Rule...**.
3. Choose **Predefined** > **Remote Desktop**.
4. Select the rules and choose **Block the connection**.

![Firewall Block Rule](./images/firewall_block_rdp.png)

---

## Activity 4 & 5: BitLocker Configuration & Recovery

**Scenario:** Encrypt the D: drive and test recovery.

### Step-by-Step Implementation:

#### Step 1: Enable BitLocker
1. Right-click the **D: drive** in File Explorer and select **Turn on BitLocker**.
2. Set a password and **Save the recovery key to a file**.

![BitLocker Setup](./images/bitlocker_setup.png)

#### Step 2: Test Recovery
1. Attempt to unlock the drive and click **More options** > **Enter recovery key**.
2. Use your saved key to unlock the drive.

![BitLocker Recovery Proof](./images/bitlocker_recovery.png)

---
*End of Activity D07 Document*

