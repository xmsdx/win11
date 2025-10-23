# Registry Key to Bypass CPU Check

**When you reach the Windows 11 setup screen:**

1. Press <kbd>Shift</kbd> + <kbd>F10</kbd> to open Command Prompt.
2. Type `regedit` and press Enter to open the Registry Editor.
3. Navigate to:  
   `HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig`  
   - If `LabConfig` does not exist, create it under `Setup`.
4. **Bypass CPU Check:**  
   - Add a new DWORD (32-bit) value:  
     - **Name:** `BypassCPUCheck`  
     - **Value:** `1`
5. **To bypass SecureBoot (optional):**  
   - Add a new DWORD (32-bit) value:  
     - **Name:** `BypassSecureBootCheck`  
     - **Value:** `1`

**Summary:**  
- **Path:** `HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig`  
- **Value:** `BypassCPUCheck` (DWORD) = 1

---

# Create a Local Account During Windows 11 Setup

1. Press <kbd>Shift</kbd> + <kbd>F10</kbd> at the account screen.
2. Disconnect from the internet.
3. (Optional) Go back to setup and click "Back" or restart the account setup—Windows will offer the option to create a local account.
4. Proceed to create a local account.

---
