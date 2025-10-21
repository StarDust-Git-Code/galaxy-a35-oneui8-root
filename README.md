# Pre-Patched One UI 8 (Android 16) Firmware for Samsung Galaxy A35 (Root / No Data Wipe)

This repository provides pre-patched firmware files to update the Samsung Galaxy A356E to One UI 8 (Android 16) **without losing data, root, or an unlocked bootloader.**

This method is based on the guide by [Star_Dust_911 on XDA-Developers](https://xdaforums.com/t/guide-flash-one-ui-8-keep-bootloader-unlock-root-data-intact.4764441/). These files were built for the **INS (India)** CSC.

**Firmware Used:**
* **New Firmware (Android 16):** `A356EXXU5CYI8`
* **Old Firmware (Android 15):** `A356EXXS5BYF3`
* **SW REV / BIT:** `5` (This method only works because both firmwares have the same bit level)

---

### **DISCLAIMER**

**You are responsible for your device.** Flashing firmware can be risky. I am not responsible for bricked devices, lost data, or any other issues. Proceed with caution.

**This will NOT work if:**
* Your bootloader is locked.
* You are on a different SW REV / Bit level.
* You have a different model of the Galaxy A35.

---

### **FEATURES**

* Updates to One UI 8 (Android 16)
* Magisk Root is preserved
* Data (`/data`) is not wiped
* Bootloader remains unlocked

---

### **DOWNLOADS**

You will need all four files from the link below.

* **[Download All 4 Firmware Files (AP, BL, CP, HOME\_CSC) from Google Drive](https://drive.google.com/drive/folders/1L1mAaq82ohDNlf0pDq5ppVapz7pwgjs_?usp=sharing)**

*(Inside the link, you will find `AP_patched.tar`, `BL_patched.tar`, `CP_...tar.md5`, and `HOME_CSC_...tar.md5`)*

---

### **HOW TO FLASH**

**1. BACKUP YOUR DATA!**
* Before you begin, use Samsung Smart Switch or another method to back up all your important data. While this method is designed to *keep* data, you must have a backup in case of failure.

**2. Boot into Download Mode:**
* Power off your Galaxy A35.
* Hold **Volume Up + Volume Down** and plug in your PC's USB-C cable.
* Press **Volume Up** to confirm.

**3. Flash with Odin:**
* Open Odin on your PC.
* Place the four files in their matching slots:
    * **BL:** `BL_patched.tar`
    * **AP:** `AP_patched.tar`
    * **CP:** `CP_A356EXXU5CYI8...`
    * **CSC:** `HOME_CSC_ODM...` (Using **HOME\_CSC** is critical to keep your data)
* In the "Options" tab, make sure **"Auto Reboot"** and **"F. Reset Time"** are checked.
* Click **Start**.

The process will take several minutes. Your phone will reboot with Android 16, root, and all your data intact.
