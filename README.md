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

Собственное приложение Vum VPN сейчас выходит для **Android** и **Windows**.
На остальных платформах подключайтесь через сторонние клиенты — ключ Vum VPN
в них работает так же.

| Платформа | Что ставим | Требования |
| --- | --- | --- |
| 🤖 **Android** — телефоны, планшеты, Android TV, в том числе 32-битные приставки | [`vum-vpn.apk`](https://github.com/vumvpn/vumvpn/releases/latest/download/vum-vpn.apk) — приложение Vum VPN | Android 7.1+ |
| 🪟 **Windows** | [`vum-vpn-setup.exe`](https://github.com/vumvpn/vumvpn/releases/latest/download/vum-vpn-setup.exe) — приложение Vum VPN | Windows 10+, x64 |
| 🍎 **iOS / iPadOS** | [Incy](https://apps.apple.com/app/incy/id6756943388) | — |
| 🖥 **macOS** | [Incy](https://apps.apple.com/app/incy/id6756943388) | — |
| 🐧 **Linux** | [Incy](https://github.com/INCY-DEV/incy-platforms/releases/latest) · [Happ](https://github.com/Happ-proxy/happ-desktop/releases/) | — |
| 🧩 **Браузер** | Расширение для [Chrome](https://chromewebstore.google.com/detail/vum-vpn/iagclfgjjpjiilcjkofbcedlpcnlkmop) и [Firefox](https://addons.mozilla.org/firefox/addon/vum-vpn/) | — |

Своего приложения для iOS, macOS и Linux пока нет. Incy ставится и из
российского App Store; Happ оттуда удалён.

Все файлы — на странице [Releases](https://github.com/vumvpn/vumvpn/releases/latest).
Подбор клиента под вашу ОС — на [vumvpn.com/install](https://vumvpn.com/install).

## Установка

<details>
<summary><b>Android</b></summary>

1. Скачайте файл `vum-vpn.apk`
2. Откройте его и разрешите установку из неизвестных источников
3. Установите приложение
4. Войдите в аккаунт и подключите VPN

> Android покажет предупреждение — это нормально для приложений не из Google Play.
> Нажмите «Всё равно установить».

На **Android TV** APK ставится так же — через файловый менеджер или приложение
Downloader. У приложения есть отдельный интерфейс под пульт.

</details>

<details>
<summary><b>Windows</b></summary>

1. Скачайте `vum-vpn-setup.exe` и запустите установщик
2. Пройдите шаги установки
3. Запустите Vum VPN — Windows спросит права администратора
4. Войдите в аккаунт или добавьте ключ и подключите VPN

> Права администратора нужны, чтобы поднять VPN-туннель. SmartScreen может
> показать предупреждение — «Подробнее» → «Выполнить в любом случае».

Крестик окна сворачивает Vum VPN в трей — VPN продолжает работать. Выйти и
отключить VPN — «Выход» в меню значка в трее.

</details>

<details>
<summary><b>iOS и macOS</b></summary>

1. Установите [**Incy**](https://apps.apple.com/app/incy/id6756943388) из App Store
2. Войдите в [личный кабинет](https://console.vumvpn.com/) и скопируйте ключ
3. Импортируйте ключ в приложение
4. Подключите VPN

</details>

<details>
<summary><b>Linux</b></summary>

1. Скачайте и установите [**Incy**](https://github.com/INCY-DEV/incy-platforms/releases/latest)
   (или [Happ](https://github.com/Happ-proxy/happ-desktop/releases/))
2. Войдите в [личный кабинет](https://console.vumvpn.com/) и скопируйте ключ
3. Импортируйте ключ в приложение
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
скорость даже при заметных потерях пакетов.

Ядро приложения на Android и Windows — [Xray](https://github.com/XTLS/Xray-core):
оно подключается ко всем нашим серверам.

## Поддержка

- 📢 Канал: [@ghostcore_vpn](https://t.me/ghostcore_vpn) — обновления и промокоды
- 💬 Чат: [@ghostcore_vpn_chat](https://t.me/ghostcore_vpn_chat)
- 🆘 Поддержка: [@ghostcore_support](https://t.me/ghostcore_support)
- 🐞 Баги и идеи: [Issues](https://github.com/vumvpn/vumvpn/issues)
- 🔐 Уязвимости: [SECURITY.md](SECURITY.md)

## Лицензия

Клиент построен на [Xray-core](https://github.com/XTLS/Xray-core) и распространяется под [GNU GPL v3.0](LICENSE).
