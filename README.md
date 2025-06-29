# 🤫🔪 QuietKill Module

QuietKill is a powerful KernelSU/Magisk module that force-kills all non-essential background apps when you lock your phone helping you **save battery**, **free RAM**, and keep your phone smooth.

> 💡 You can [whitelist](#-ignore-list-format) apps you don't want to kill (like WhatsApp or Telegram) by adding them to an ignore list.

## 🧠 What It Does

- ✅ Force-stops all **user apps**
- ✅ Supports force-killing **specific system apps**
- ✅ **Ignore list (whitelist mode)** to protect key apps
- ✅ **Force Kill List** for system apps to always kill on lock
- ✅ **WebUI** to control force-stops, manage lists, and view logs
- ✅ **Power Key = Kill**: Automatically triggers on screen lock

<div align="center">
  <a href="https://github.com/TempMeow/QuietKill/releases" target="_blank">
    <img src="media/download.png" alt="Download Button" width="600" />
  </a>
</div>


## Preview
![QuietKill Demo](https://github.com/TempMeow/QuietKill/blob/4403642b2b9547da316cec5207dce64e1a27e8e8/media/1.gif)


## 🛠️ How to Use

### 1. Install the Module
- Flash via **Magisk**, **KernelSU**, or **A-Patch**
- Reboot your device

### 2. Kill Apps Automatically (Power Key = Kill)
- Press the **power button to lock your screen**
- QuietKill instantly runs & kills all background running apps
- Add your apps to the **ignore list** to keep them alive
- Add system apps to the **force kill list** to *ensure* they are killed every time


## 📃 Ignore List Format

File location:
```
$MODDIR/ignore.txt
```

Use this list to protect apps you **don’t want killed**.

Example:
```
com.whatsapp
com.google.android.gms
```

Each line = one app package to **ignore from being killed**.


## 🔥 Force Kill List Format (System Apps)

File location:
```
$MODDIR/ForceKill.txt
```

Use this list to **force-kill specific system apps** (e.g., bloatware or system services) on **every lockscreen trigger**.

Example:
```
com.google.android.gms
com.miui.analytics
```

Each line = one **system app** package to be killed even if normally ignored.

> ⚠️ Use with caution killing essential system apps can lead to instability.


## 🌐 WebUI Features

- Start/stop kill actions manually
- View kill logs in real time
- Manage **ignore list** and **force kill list**

## ⚠️ Disclaimer

Force-killing apps may break notifications, background sync, or alarms.  
Use the **ignore list** for critical apps (e.g., messaging, banking, health apps).  
Be careful with the **force kill list** killing system apps can cause unexpected behavior.


## 📦 Optional: Download Toast Generator

<p align="center">
  <a href="https://github.com/TempMeow/QuietKill/releases/download/v1/Toaster.apk">
    <img src="https://img.shields.io/badge/Download-APK-blue?style=for-the-badge&logo=android" alt="Download APK"/>
  </a>
</p>


Made with ❤️ by [Mona](https://t.me/TempMeow)
