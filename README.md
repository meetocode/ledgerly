# Ledgerly

Personal finance monitoring. Your data stays on your device, encrypted.

## Download

| Platform | Download |
|---|---|
| Windows (installer) | [Ledgerly-Setup.exe](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-Setup.exe) |
| Windows (portable) | [Ledgerly-windows-x64.zip](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-windows-x64.zip) |
| Linux x64 | [Ledgerly-linux-x64.tar.gz](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-linux-x64.tar.gz) |
| iPhone (unsigned, for sideloading) | [Ledgerly-unsigned.ipa](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-unsigned.ipa) |

Older versions and release notes: [Releases](https://github.com/meetocode/ledgerly/releases).

## Windows

1. Download and run **Ledgerly-Setup.exe**. No administrator rights are needed.
2. Ledgerly isn't code-signed yet, so Windows may show **"Windows protected your PC"**. Click **More info**, then **Run anyway**.
3. Installing a newer version over an older one keeps your data.

**Uninstalling deletes your data.** Uninstalling Ledgerly (Settings › Apps) permanently deletes all Ledgerly data on the computer, including every user's ledger, after asking you to confirm. Your Recovery Key can't bring it back.

The portable zip needs no install: unzip it and run `ledgerly.exe`. It uses the same data folder, `%APPDATA%\Ledgerly\Ledgerly`.

## Linux

```sh
sudo apt install libgtk-3-0 libssl3      # Debian / Ubuntu
mkdir ledgerly && tar -xzf Ledgerly-linux-x64.tar.gz -C ledgerly
./ledgerly/ledgerly
```

Your data is in `~/.local/share/app.ledgerly.ledgerly/`. Delete that folder to remove it.

## iPhone

The iPhone build isn't on the App Store. You install it from a Windows or Mac computer with [Sideloadly](https://sideloadly.io/), which signs it with your own Apple ID.

1. Install Sideloadly and connect your iPhone with a USB cable.
2. Drag **Ledgerly-unsigned.ipa** into Sideloadly. Sign in with your Apple ID (an [app-specific password](https://support.apple.com/102654) is recommended) and click **Start**.
   If it complains about the bundle ID, enable Sideloadly's option to change it.
3. On the iPhone: **Settings › General › VPN & Device Management**, trust your Apple ID's developer profile. Then turn on **Settings › Privacy & Security › Developer Mode** and restart when asked.
4. **With a free Apple ID the app stops opening after 7 days.** Install it again the same way. Installing over the existing app keeps your data, but deleting the app deletes its data.

## Licence

Free to use. See [LICENSE](LICENSE). The source code isn't public.
