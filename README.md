

# Welcome to Debian Linux Guide for Beginners 🚀

This guide is made for beginners who want to start using **Debian Linux** easily.  
Just copy and paste the commands into your terminal.  

---

## 📥 Downloading Debian ISO

Debian offers different installation images:

- **Netboot (Minimal Install):**  
  👉 [https://www.debian.org/distrib/netinst](https://www.debian.org/distrib/netinst)

- **GNOME Desktop (Default):**  
  👉 [https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/](https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/)

- **KDE Plasma Desktop:**  
  👉 [https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/](https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/)

- **Other Desktops (XFCE, LXDE, Cinnamon, MATE, etc.):**  
  👉 [https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/](https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/)

---

## 💻 Setting up a Virtual Machine

- **VirtualBox (Free & Open Source):**  
  👉 [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)

- **VMware Workstation Player (Free for Personal Use):**  
  👉 [https://www.vmware.com/products/workstation-player.html](https://www.vmware.com/products/workstation-player.html)

After downloading, create a new VM and attach the Debian ISO.

---

## 🔑 First Boot & Update

Once Debian is installed, update your system:

```bash
sudo apt update && sudo apt upgrade -y
````
---
## 📦 Backup / Snapshot of System

Once Debian is installed, Make sure take a snapshot of system to incase of messing something up.
i'll suggest TimeShift to take backup.
```bash
sudo add-apt-repository -y ppa:teejee2008/timeshift
sudo apt-get update
sudo apt-get install timeshift
````
---

## 🔎 Searching for an Application

Example: Searching for **VLC** or **Chrome**:

```bash
sudo apt search vlc
sudo apt search chrome
```

---

## 🎥 Installing a Video Player

Install **VLC** and **MPV**:

```bash
sudo apt install vlc mpv -y
```

---

## 📂 Installing a File Manager

Here are some popular file managers you can install:

* **Dolphin (KDE):**

  ```bash
  sudo apt install dolphin -y
  ```

* **Nautilus (GNOME default):**

  ```bash
  sudo apt install nautilus -y
  ```

* **Thunar (XFCE):**

  ```bash
  sudo apt install thunar -y
  ```

* **PCManFM (LXDE / Lightweight):**

  ```bash
  sudo apt install pcmanfm -y
  ```

* **Caja (MATE):**

  ```bash
  sudo apt install caja -y
  ```

---

## 📦 Installing `.deb` Packages

Sometimes you download software in `.deb` format (like Google Chrome, VS Code, Zoom).

1. Install with `dpkg`:

   ```bash
   sudo dpkg -i package-name.deb
   ```

2. Fix missing dependencies:

   ```bash
   sudo apt --fix-broken install -y
   ```

---

## 📂 Working with Archives

### Extracting `.tar.gz` / `.tar.xz`:

```bash
tar -xvzf file.tar.gz
tar -xvJf file.tar.xz
```

### Creating a tarball:

```bash
tar -cvzf archive.tar.gz foldername/
```

---

### Zip & Unzip

* Install zip tools:

  ```bash
  sudo apt install zip unzip -y
  ```
* Create a zip:

  ```bash
  zip myarchive.zip file1 file2
  ```
* Extract a zip:

  ```bash
  unzip myarchive.zip
  ```

---

### RAR & UnRAR

* Install:

  ```bash
  sudo apt install rar unrar -y
  ```
* Create rar:

  ```bash
  rar a archive.rar file1 file2
  ```
* Extract rar:

  ```bash
  unrar x archive.rar
  ```

---

### GUI Archivers (Easy File Extraction)

* **PeaZip (Powerful GUI Archive Manager):**

  ```bash
  sudo apt install peazip -y
  ```

* **Xarchiver (Lightweight GUI):**

  ```bash
  sudo apt install xarchiver -y
  ```

---

## 📘 Tools for Students & Office Use

### Office Suites

* **LibreOffice (Full Office Suite):**

  ```bash
  sudo apt install libreoffice -y
  ```

* **OnlyOffice (MS Office Alternative):**

  ```bash
  sudo apt install onlyoffice-desktopeditors -y
  ```

### Note Taking

* **Joplin (Notes + To-Do):**

  ```bash
  sudo apt install joplin -y
  ```

* **Zim Wiki (Personal Wiki Notes):**

  ```bash
  sudo apt install zim -y
  ```

### PDF Tools

* **Okular (View & Annotate PDFs):**

  ```bash
  sudo apt install okular -y
  ```

* **Evince (Lightweight PDF Reader):**

  ```bash
  sudo apt install evince -y
  ```

### Programming Tools

* **VS Code (Popular IDE):**
  Download `.deb` 👉 [https://code.visualstudio.com/Download](https://code.visualstudio.com/Download)
  Then install:

  ```bash
  sudo dpkg -i code*.deb
  sudo apt --fix-broken install -y
  ```

* **Git (Version Control):**

  ```bash
  sudo apt install git -y
  ```

---
## Running Windows Apps on Linux
you can set this apps to setting up win apps on linux 
```
https://github.com/winapps-org/winapps
https://github.com/TibixDev/winboat
````
---

## ✅ Quick Tips

* Shutdown the system:

  ```bash
  sudo poweroff
  ```
  ```bash
  sudo shutdown now
  ```

* Reboot the system:

  ```bash
  sudo reboot
  ```
* Check CPU usage:

  ```bash
  top
  ```
  ```bash
  htop
  ```
    ```bash
  btop
  ```
* Check disk space:

  ```bash
  df -h
  ```

* Check memory usage:

  ```bash
  free -h
  ```

---

🎉 Congratulations! You now have a working Debian system with **apps, archive tools, and productivity software**.
