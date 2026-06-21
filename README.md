# Custom Windows 11 Boot Logo

Customize your Windows 11 boot logo with your own image using **HackBGRT**.

> **Disclaimer:** This project is for educational and personalization purposes only. All trademarks, logos, and copyrights belong to their respective owners.

## Prerequisites

* Windows 11 installed in **UEFI** mode
* Administrator access
* Secure Boot disabled

---

## Step 1: Verify UEFI Mode

1. Press **Win + R**
2. Type `msinfo32` and press **Enter**
3. Check **BIOS Mode**
4. Ensure it shows **UEFI**

---

## Step 2: Disable Secure Boot

1. Hold **Shift** and click **Restart**

2. Navigate to:

   `Troubleshoot → Advanced Options → UEFI Firmware Settings → Restart`

3. In your motherboard/UEFI settings:

   * Locate **Secure Boot**
   * Disable it

4. Save changes (**F10** on most systems) and reboot

---

## Step 3: Prepare Your Boot Logo

1. Open your image in the **Photos** app

2. Select **Resize**

3. Set dimensions to:

   * Width: **250 px**
   * Height: **250 px**

4. Save the image as:

   ```text
   splash.bmp
   ```

> The filename and extension must match exactly.

---

## Step 4: Install HackBGRT

Download the latest release:

**HackBGRT Repository:**
https://github.com/Metabolix/HackBGRT/releases

### Installation

1. Extract the downloaded ZIP

2. Run `setup.exe` as Administrator

3. Press **I** to install

4. When the configuration Notepad opens, simply close it

5. MS Paint will open automatically

6. Open:

   ```text
   SYSTEM (A:) → EFI → HackBGRT → splash.bmp
   ```

7. Replace it with your custom `splash.bmp`

8. Save and close Paint

9. Close the command window

---

## Step 5: Reboot

Restart your PC and enjoy your custom Windows boot logo.

---

## Rollback / Restore Default Logo

If you want to revert all changes:

1. Open the HackBGRT folder
2. Run `setup.exe`
3. Press **R** to remove HackBGRT completely
4. Restart your system

Your default Windows boot logo will be restored.

---

## Notes

* Works only on **UEFI-based systems**
* Secure Boot must remain disabled while using HackBGRT
* Always keep a backup before modifying EFI settings

## License

This repository provides guidance only. Users are responsible for any changes made to their systems.
