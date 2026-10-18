<p align="center">
  <img src="assets/logo.svg" width="88" alt="" />
</p>

<h1 align="center">Vum VPN</h1>

<p align="center">
  <strong>A fast VPN your ISP and DPI boxes can't see</strong>
</p>

<p align="center">
  <a href="https://vumvpn.com">Website</a> ·
  <a href="https://console.vumvpn.com/">Console</a> ·
  <a href="https://github.com/vumvpn/vumvpn/releases/latest">Download</a> ·
  <a href="https://t.me/ghostcore_vpn">Telegram</a> ·
  <a href="README.md">Русский</a>
</p>

---

This repository hosts **app builds and setup guides**. Keys, plans and billing
live in the [console](https://console.vumvpn.com/); the client and server
source code is in a private repository.

## Download

The Vum VPN app itself currently ships for **Android** and **Windows**. On other
platforms, connect with a third-party client — your Vum VPN key works there the
same way.

| Platform | What to install | Requirements |
| --- | --- | --- |
| 🤖 **Android** — phones, tablets, Android TV, including 32-bit TV boxes | [`vum-vpn.apk`](https://github.com/vumvpn/vumvpn/releases/latest/download/vum-vpn.apk) — the Vum VPN app | Android 7.1+ |
| 🪟 **Windows** | [`vum-vpn-setup.exe`](https://github.com/vumvpn/vumvpn/releases/latest/download/vum-vpn-setup.exe) — the Vum VPN app, [see the limitation below](#windows-limitation) · [Incy](https://github.com/INCY-DEV/incy-platforms/releases/latest) | Windows 10+, x64 |
| 🍎 **iOS / iPadOS** | [Incy](https://apps.apple.com/app/incy/id6756943388) | — |
| 🖥 **macOS** | [Incy](https://apps.apple.com/app/incy/id6756943388) | — |
| 🐧 **Linux** | [Incy](https://github.com/INCY-DEV/incy-platforms/releases/latest) · [Happ](https://github.com/Happ-proxy/happ-desktop/releases/) | — |
| 🧩 **Browser** | Extension for [Chrome](https://chromewebstore.google.com/detail/vum-vpn/iagclfgjjpjiilcjkofbcedlpcnlkmop) and [Firefox](https://addons.mozilla.org/firefox/addon/vum-vpn/) | — |

<a id="windows-limitation"></a>
> **Windows: a limitation of the current version.** The Windows app still runs on
> the sing-box core, while our VLESS + Reality servers only accept a recent Xray.
> So Hysteria2 servers connect in it, but Reality servers don't. Moving the
> Windows app to Xray is in progress; until then, use Incy for all servers.

There is no Vum VPN app for iOS, macOS or Linux yet. Incy is available in the
Russian App Store too; Happ has been removed from it.

Every file lives on the [Releases](https://github.com/vumvpn/vumvpn/releases/latest)
page. Pick a client for your OS at [vumvpn.com/install](https://vumvpn.com/install).

## Installation

<details>
<summary><b>Android</b></summary>

1. Download `vum-vpn.apk`
2. Open it and allow installation from unknown sources
3. Install the app
4. Sign in and connect the VPN

> Android will warn you — that's normal for apps installed outside Google Play.
> Tap "Install anyway".

On **Android TV** the APK installs the same way — via a file manager or the
Downloader app. The app has a separate remote-friendly interface.

</details>

<details>
<summary><b>Windows</b></summary>

1. Download `vum-vpn-setup.exe` and run the installer
2. Follow the installation steps
3. Launch Vum VPN **as administrator**
4. Add your key and connect the VPN

> Administrator rights are required to create the VPN tunnel. SmartScreen may
> show a warning — click "More info" → "Run anyway".

While the Windows app is on sing-box, VLESS + Reality servers don't connect in it —
[details](#windows-limitation). For those, install
[Incy for Windows](https://github.com/INCY-DEV/incy-platforms/releases/latest)
and import your key as in the Linux guide below.

</details>

<details>
<summary><b>iOS and macOS</b></summary>

1. Install [**Incy**](https://apps.apple.com/app/incy/id6756943388) from the App Store
2. Sign in to the [console](https://console.vumvpn.com/) and copy your key
3. Import the key into the app
4. Connect the VPN

</details>

<details>
<summary><b>Linux</b></summary>

1. Download and install [**Incy**](https://github.com/INCY-DEV/incy-platforms/releases/latest)
   (or [Happ](https://github.com/Happ-proxy/happ-desktop/releases/))
2. Sign in to the [console](https://console.vumvpn.com/) and copy your key
3. Import the key into the app
4. Connect the VPN

</details>

## How to use it

1. **Get a key.** Open [console.vumvpn.com](https://console.vumvpn.com/) or the
   [@ghostcore_vpn_bot](https://t.me/ghostcore_vpn_bot) bot, sign in and pick a plan.
2. **Add the key to the app.** In the client tap "+" → scan the QR code or paste
   the subscription link from your clipboard.
3. **Connect.** The big button on the main screen. That's it.

A key is a subscription link: the servers behind it refresh on their own, so you
never have to re-import anything. One key works on several devices.

## Protocols

**VLESS + Reality** disguises traffic as ordinary HTTPS — to an ISP or a DPI box
it looks like a visit to a regular website. **Hysteria2** is UDP over QUIC and
holds its speed even with noticeable packet loss.

The Android app runs on the [Xray](https://github.com/XTLS/Xray-core) core, which
connects to all of our servers. The Windows app is still on
[sing-box](https://github.com/SagerNet/sing-box) and is moving to Xray.

## Support

- 📢 Channel: [@ghostcore_vpn](https://t.me/ghostcore_vpn) — updates and promo codes
- 💬 Chat: [@ghostcore_vpn_chat](https://t.me/ghostcore_vpn_chat)
- 🆘 Support: [@ghostcore_support](https://t.me/ghostcore_support)
- 🐞 Bugs and ideas: [Issues](https://github.com/vumvpn/vumvpn/issues)
- 🔐 Vulnerabilities: [SECURITY.md](SECURITY.md)

## License

The client is built on [Xray-core](https://github.com/XTLS/Xray-core) (Android) and
[sing-box](https://github.com/SagerNet/sing-box) (Windows) and is distributed under the [GNU GPL v3.0](LICENSE).
