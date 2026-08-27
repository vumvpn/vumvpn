<p align="center">
  <img src="assets/logo.svg" width="88" alt="" />
</p>

<h1 align="center">Vum VPN</h1>

<p align="center">
  <strong>Быстрый VPN, который не видно ни провайдеру, ни DPI</strong>
</p>

<p align="center">
  <a href="https://vumvpn.com">Сайт</a> ·
  <a href="https://console.vumvpn.com/">Личный кабинет</a> ·
  <a href="https://github.com/vumvpn/vumvpn/releases/latest">Скачать</a> ·
  <a href="https://t.me/ghostcore_vpn">Telegram</a> ·
  <a href="README.en.md">English</a>
</p>

---

Здесь живут **сборки приложений и инструкции**. Ключи, тарифы и оплата — в
[личном кабинете](https://console.vumvpn.com/); исходный код клиента и
серверной части — в закрытом репозитории.

## Скачать

| Платформа | Что ставим | Требования |
| --- | --- | --- |
| 🤖 **Android** | [`vum-vpn.apk`](https://github.com/vumvpn/vumvpn/releases/latest) | Android 7.0+ |
| 🪟 **Windows** | [`vum-vpn-setup.exe`](https://github.com/vumvpn/vumvpn/releases/latest) | Windows 10+ |
| 🍎 **iOS** | [Happ](https://apps.apple.com/by/app/happ-proxy-utility/id6504287215) · [Incy](https://apps.apple.com/app/incy/id6756943388) (для российского App Store) | iOS 15+ |
| 🖥 **macOS** | [Happ](https://apps.apple.com/by/app/happ-proxy-utility/id6504287215) · [Incy](https://apps.apple.com/app/incy/id6756943388) | macOS 12+ |
| 🐧 **Linux** | [Happ](https://github.com/aspect-build/happ/releases/latest) | — |
| 🌐 **Браузер** | [console.vumvpn.com](https://console.vumvpn.com/) — работает как PWA | любой |

Все файлы — на странице [Releases](https://github.com/vumvpn/vumvpn/releases/latest).
Зеркало и подбор платформы по вашей ОС — на [vumvpn.com/install](https://vumvpn.com/install).

## Установка

<details>
<summary><b>Android</b></summary>

1. Скачайте файл `vum-vpn.apk`
2. Откройте его и разрешите установку из неизвестных источников
3. Установите приложение
4. Войдите в аккаунт и подключите VPN

> Android покажет предупреждение — это нормально для приложений не из Google Play.
> Нажмите «Всё равно установить».

</details>

<details>
<summary><b>Windows</b></summary>

1. Скачайте `vum-vpn-setup.exe` и запустите установщик
2. Пройдите шаги установки
3. Запустите Vum VPN **от имени администратора**
4. Добавьте ключ и подключите VPN

> Права администратора нужны, чтобы поднять VPN-туннель. SmartScreen может
> показать предупреждение — «Подробнее» → «Выполнить в любом случае».

</details>

<details>
<summary><b>iOS и macOS</b></summary>

1. Установите **Happ** из App Store (или **Incy**, если ваш App Store — Россия)
2. Войдите в [личный кабинет](https://console.vumvpn.com/) и скопируйте ключ
3. Импортируйте ключ в приложение
4. Подключите VPN

</details>

<details>
<summary><b>Linux</b></summary>

1. Скачайте и установите **Happ**
2. Войдите в [личный кабинет](https://console.vumvpn.com/) и скопируйте ключ
3. Импортируйте ключ в Happ
4. Подключите VPN

</details>

## Как пользоваться

1. **Получите ключ.** Откройте [console.vumvpn.com](https://console.vumvpn.com/)
   или бот [@ghostcore_vpn_bot](https://t.me/ghostcore_vpn_bot), войдите и
   выберите тариф.
2. **Добавьте ключ в приложение.** В клиенте — «+» → отсканировать QR-код или
   вставить ссылку подписки из буфера обмена.
3. **Подключитесь.** Большая кнопка на главном экране. Готово.

Ключ — это ссылка-подписка: серверы в ней обновляются сами, переподключать
ничего не нужно. Один ключ работает на нескольких устройствах.

## Протоколы

**VLESS + Reality** — маскирует трафик под обычный HTTPS: для провайдера и
DPI-систем это визит на обычный сайт. **Hysteria2** — UDP поверх QUIC, держит
скорость даже при заметных потерях пакетов. Под капотом — [sing-box](https://github.com/SagerNet/sing-box).

## Поддержка

- 📢 Канал: [@ghostcore_vpn](https://t.me/ghostcore_vpn) — обновления и промокоды
- 💬 Чат: [@ghostcore_vpn_chat](https://t.me/ghostcore_vpn_chat)
- 🆘 Поддержка: [@ghostcore_support](https://t.me/ghostcore_support)
- 🐞 Баги и идеи: [Issues](https://github.com/vumvpn/vumvpn/issues)
- 🔐 Уязвимости: [SECURITY.md](SECURITY.md)

## Лицензия

Клиент построен на [sing-box](https://github.com/SagerNet/sing-box) и
распространяется под [GNU GPL v3.0](LICENSE).
