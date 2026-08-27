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

| Platform | What to install | Requirements |
| --- | --- | --- |
| 🤖 **Android** | [`vum-vpn.apk`](https://github.com/vumvpn/vumvpn/releases/latest) | Android 7.0+ |
| 🪟 **Windows** | [`vum-vpn-setup.exe`](https://github.com/vumvpn/vumvpn/releases/latest) | Windows 10+ |
| 🍎 **iOS** | [Happ](https://apps.apple.com/by/app/happ-proxy-utility/id6504287215) · [Incy](https://apps.apple.com/app/incy/id6756943388) (for the Russian App Store) | iOS 15+ |
| 🖥 **macOS** | [Happ](https://apps.apple.com/by/app/happ-proxy-utility/id6504287215) · [Incy](https://apps.apple.com/app/incy/id6756943388) | macOS 12+ |
| 🐧 **Linux** | [Happ](https://github.com/aspect-build/happ/releases/latest) | — |
| 🌐 **Browser** | [console.vumvpn.com](https://console.vumvpn.com/) — installable as a PWA | any |

Every file lives on the [Releases](https://github.com/vumvpn/vumvpn/releases/latest)
page. A mirror that picks the build for your OS: [vumvpn.com/install](https://vumvpn.com/install).

## Installation

<details>
<summary><b>Android</b></summary>

1. Download `vum-vpn.apk`
2. Open it and allow installation from unknown sources
3. Install the app
4. Sign in and connect the VPN

> Android will warn you — that's normal for apps installed outside Google Play.
> Tap "Install anyway".

</details>

<details>
<summary><b>Windows</b></summary>

1. Download `vum-vpn-setup.exe` and run the installer
2. Follow the installation steps
3. Launch Vum VPN **as administrator**
4. Add your key and connect the VPN

> Administrator rights are required to create the VPN tunnel. SmartScreen may
> show a warning — click "More info" → "Run anyway".

</details>

<details>
<summary><b>iOS and macOS</b></summary>

1. Install **Happ** from the App Store (or **Incy** if your App Store region is Russia)
2. Sign in to the [console](https://console.vumvpn.com/) and copy your key
3. Import the key into the app
4. Connect the VPN

</details>

<details>
<summary><b>Linux</b></summary>

1. Download and install **Happ**
2. Sign in to the [console](https://console.vumvpn.com/) and copy your key
3. Import the key into Happ
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
holds its speed even with noticeable packet loss. Powered by
[sing-box](https://github.com/SagerNet/sing-box).

## Support

- 📢 Channel: [@ghostcore_vpn](https://t.me/ghostcore_vpn) — updates and promo codes
- 💬 Chat: [@ghostcore_vpn_chat](https://t.me/ghostcore_vpn_chat)
- 🆘 Support: [@ghostcore_support](https://t.me/ghostcore_support)
- 🐞 Bugs and ideas: [Issues](https://github.com/vumvpn/vumvpn/issues)
- 🔐 Vulnerabilities: [SECURITY.md](SECURITY.md)

## License

The client is built on [sing-box](https://github.com/SagerNet/sing-box) and is
distributed under the [GNU GPL v3.0](LICENSE).
