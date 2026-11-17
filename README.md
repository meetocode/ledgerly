<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.svg">
  <img src="assets/logo-light.svg" alt="Ledgerly" width="444">
</picture>

<h3>Every cent, accounted for.</h3>

A private personal finance tracker for Windows, Linux and iPhone.<br>
Your ledger lives on your device. No email, no cloud account.

<a href="https://github.com/meetocode/ledgerly/releases/latest"><img src="https://img.shields.io/github/v/release/meetocode/ledgerly?style=flat&label=release&color=087F6E" alt="Latest release"></a>
<img src="https://img.shields.io/badge/platforms-Windows%20%C2%B7%20Linux%20%C2%B7%20iPhone-56657D?style=flat" alt="Platforms: Windows, Linux, iPhone">
<a href="LICENSE"><img src="https://img.shields.io/badge/licence-free%20to%20use-56657D?style=flat" alt="Licence: free to use"></a>

</div>

## Download

[Release notes](https://github.com/meetocode/ledgerly/releases/latest) · [All releases](https://github.com/meetocode/ledgerly/releases)

<p>
  <a href="https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-Setup.exe"><img src="assets/download-windows.svg" alt="Download for Windows" width="272"></a>
  <a href="https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-linux-x64.tar.gz"><img src="assets/download-linux.svg" alt="Download for Linux" width="272"></a>
  <a href="https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-unsigned.ipa"><img src="assets/download-iphone.svg" alt="Download for iPhone" width="272"></a>
</p>

| | Platform | File | What it is |
|:-:|---|---|---|
| <img src="assets/icon-windows.svg" width="20" alt=""> | **Windows** | [`Ledgerly-Setup.exe`](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-Setup.exe) | Installer. No administrator rights needed. |
| <img src="assets/icon-windows.svg" width="20" alt=""> | **Windows** | [`Ledgerly-windows-x64-portable.zip`](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-windows-x64-portable.zip) | Portable. Unzip and run, nothing to install. |
| <img src="assets/icon-linux.svg" width="20" alt=""> | **Linux** | [`Ledgerly-linux-x64.tar.gz`](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-linux-x64.tar.gz) | 64-bit build for Debian, Ubuntu and similar. |
| <img src="assets/icon-apple.svg" width="20" alt=""> | **iPhone** | [`Ledgerly-unsigned.ipa`](https://github.com/meetocode/ledgerly/releases/latest/download/Ledgerly-unsigned.ipa) | Unsigned app. Install it with Sideloadly. |

## What's coming

Ledgerly 0.0.x is an early preview. These are on the way:

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/features-dark.svg">
  <img src="assets/features-light.svg" alt="Coming to Ledgerly: see where you stand; income against spending; spending by category; every account in one place; subscriptions and debit orders; investments; find anything fast with Ctrl K; your currency; light or dark; private by design" width="880">
</picture>

## Install

### Windows

1. Download and run `Ledgerly-Setup.exe`. No administrator rights are needed.
2. Ledgerly isn't code-signed yet, so Windows may show "Windows protected your PC". Click **More info**, then **Run anyway**.
3. Installing a newer version over an older one keeps your data.
4. From 0.0.2 on, the installed app keeps itself up to date: it checks once a day (you can turn this off in Settings › About), downloads the update, checks it is genuine, and installs it when you restart or close Ledgerly. The portable zip, Linux and iPhone builds tell you when an update is out and link here.

> [!WARNING]
> **Uninstalling deletes your data.** Uninstalling Ledgerly (Settings › Apps) permanently deletes all Ledgerly data on the computer, including every user's ledger, after asking you to confirm. Your Recovery Key can't bring it back.

The portable zip needs no install: unzip it and run `ledgerly.exe`. It uses the same data folder, `%APPDATA%\Ledgerly\Ledgerly`.

### Linux

```bash
sudo apt install libgtk-3-0 libssl3      # Debian / Ubuntu
mkdir ledgerly && tar -xzf Ledgerly-linux-x64.tar.gz -C ledgerly
./ledgerly/ledgerly
```

Your data is in `~/.local/share/app.ledgerly.ledgerly/`. Delete that folder to remove it.

### iPhone

The iPhone build isn't on the App Store. You install it from a Windows or Mac computer with [Sideloadly](https://sideloadly.io/), which signs it with your own Apple ID.

1. Install Sideloadly and connect your iPhone with a USB cable.
2. Drag `Ledgerly-unsigned.ipa` into Sideloadly. Sign in with your Apple ID (an [app-specific password](https://support.apple.com/102654) is recommended) and click **Start**. If it complains about the bundle ID, enable Sideloadly's option to change it.
3. On the iPhone: **Settings › General › VPN & Device Management**, trust your Apple ID's developer profile. Then turn on **Settings › Privacy & Security › Developer Mode** and restart when asked.
4. With a free Apple ID the app stops opening after 7 days. Install it again the same way.

> [!IMPORTANT]
> Installing over the existing app keeps your data, but deleting the app deletes its data.

## Licence

Free to use. See [LICENSE](LICENSE). The source code isn't public.
