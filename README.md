# 💣 QuietKill Module

QuietKill is a powerful KernelSU/Magisk module that force-kills all non-essential background apps in one tap or with a volume button trigger to help you **save battery**, **free RAM**, and keep your phone smooth.

> 💡 You can [whitelist](https://github.com/TempMeow/QuietKill/blob/main/README.md#-ignore-list-format) apps you don't want to kill (like WhatsApp or Telegram) by adding them to an ignore list.



## 🧠 What It Does

- ✅ Force-stops all **user apps**
- ✅ Includes default system apps like **Play Store & Play Services**
- ✅ **Ignore list** to exclude important apps
- ✅ **WebUI** to control everything (force-stop, view logs, add/remove ignore apps)
- ✅ **Volume Key Trigger**: triple-press volume up to kill apps from anywhere

<div align="center">
  <a href="https://github.com/TempMeow/QuietKill/releases" target="_blank">
    <img src="media/download.png" alt="Download Button" width="600" />
  </a>
</div>

## Preview
![QuietKill Demo](https://github.com/TempMeow/QuietKill/blob/4403642b2b9547da316cec5207dce64e1a27e8e8/media/1.gif)

## 🛠️ How to Use

### 1. Install the Module
- Flash the module via **Magisk**, **KernelSU**, or **A-Patch**
- Reboot your device

### 2. Kill Apps (Two Methods – Use Either)

#### 🔘 Method 1: Use the WebUI
- Open the WebUI
- Tap **"Force Stop Apps"**
- View logs in the **terminal-style output**
- Add apps to the ignore list to keep them running

#### 🔊 Method 2: Use Volume-Up Trigger
- Triple-press the **Volume Up** button (from anywhere)
- The script runs silently in the background
- Toggle listener on/off using the `/sdcard/stopQuietKill` file



## 🧾 Ignore List Format

File location:
```
$MODDIR/ignore.txt
```

Example contents:
```
com.whatsapp
com.google.android.gms
```

Each line = one app package to **ignore from being killed**.



## 🛑 Toggle Volume Trigger (Enable/Disable)
```bash
✅ Use the action button in your root manager

# 🔕 Disable the volume trigger
touch /sdcard/stopQuietKill

# 🔔 Re-enable the volume trigger
rm /sdcard/stopQuietKill
```

## ⚠️ Disclaimer

Force-killing apps may break notifications or background services.  
Always use the **ignore list** to exclude apps you rely on (like messaging or banking).


Made with love by [Mona](https://t.me/MeowDump)
