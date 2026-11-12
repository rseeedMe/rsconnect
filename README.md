<h1 align="center">Ryse</h1>

<p align="center"><b>Кроссплатформенный VPN-клиент на базе <a href="https://github.com/XTLS/Xray-core">Xray-core</a></b></p>

<p align="center">
  <a href="https://github.com/rseeedMe/rsconnect/releases"><img alt="Релизы" src="https://img.shields.io/badge/Releases-GitHub-181717?logo=github"></a>
  <a href="https://github.com/rseeedMe/rsconnect/releases/latest"><img alt="Последняя версия" src="https://img.shields.io/github/v/release/rseeedMe/rsconnect?label=Version&color=22C55E"></a>
  <a href="https://rs-connect-1.gitbook.io/rs-connect-docs/"><img alt="Документация" src="https://img.shields.io/badge/Docs-GitBook-3884FF?logo=gitbook&logoColor=white"></a>
</p>

## Загрузки

Ссылки всегда ведут на последнюю версию. Все версии и список изменений: [Releases](https://github.com/rseeedMe/rsconnect/releases).
Контрольные суммы файлов каждого релиза: `SHA256SUMS.txt`.

### Компьютер

| Платформа | Установщик | Портативная версия |
|---|---|---|
| Windows (x64) | [Setup](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-windows-x64-setup.exe) | [ZIP](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-windows-x64.zip) |
| macOS (Apple Silicon и Intel, один файл) | [DMG](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-macos.dmg) | [ZIP](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-macos.zip) |
| Windows (ARM64) | тот же Setup: работает через встроенную эмуляцию x64 | тот же ZIP |
| Linux (x64) | в разработке | в разработке |

### Телефоны и ТВ

| Платформа | Ссылка |
|---|---|
| Android (телефоны и планшеты, arm64) | [APK](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-android-arm64.apk) |
| Android (эмулятор, x86_64) | [APK](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-android-x86_64.apk) |
| Google Play | готовится |
| Android TV и приставки (arm64) | тот же [APK](https://github.com/rseeedMe/rsconnect/releases/latest/download/Ryse-android-arm64.apk): управление пультом, подписка по коду от провайдера |
| iOS / Apple TV | в разработке |

> [!NOTE]
> **Windows.** SmartScreen может предупредить о неизвестном издателе: нажмите «Подробнее» → «Выполнить в любом случае».
>
> **macOS.** При первом запуске система сообщит, что приложение от неустановленного разработчика: откройте
> Системные настройки → Конфиденциальность и безопасность и нажмите «Всё равно открыть».
>
> **Android.** При установке APK разрешите установку из этого источника (браузера). При первом подключении
> система спросит разрешение на VPN.
>
> На всех платформах установленное приложение обновляется само: Настройки → О приложении → «Установить».

## Установка

**Windows**

1. Скачайте Setup и запустите, нажмите «Далее».
2. Откройте Ryse и вставьте ссылку подписки от вашего провайдера, или нажмите кнопку «Добавить в приложение» у провайдера.
3. Нажмите «Подключить VPN». Сервер выберется автоматически, при желании выберите страну вручную.

**macOS**

1. Скачайте DMG, откройте его и перетащите Ryse в папку «Программы».
2. Запустите приложение из «Программ». Если macOS не даёт открыть, разрешите запуск в Системные настройки → Конфиденциальность и безопасность → «Всё равно открыть».
3. Добавьте подписку и нажмите «Подключить VPN». Режим TUN один раз попросит пароль администратора.

**Android**

1. Скачайте APK прямо на телефоне и откройте его из уведомления о загрузке.
2. Запустите Ryse, добавьте подписку (плюс справа вверху → вставить ссылку).
3. Нажмите «Подключить VPN» и подтвердите запрос системы. Пока VPN работает, в шторке висит уведомление с кнопкой «Отключить».

Подробнее: [документация](https://rs-connect-1.gitbook.io/rs-connect-docs/).

## Протоколы

![VLESS](https://img.shields.io/badge/VLESS-Reality%20%C2%B7%20XHTTP-4ADE80) ![VMess](https://img.shields.io/badge/VMess-4ADE80) ![Trojan](https://img.shields.io/badge/Trojan-4ADE80) ![Shadowsocks](https://img.shields.io/badge/Shadowsocks-4ADE80) ![Hysteria2](https://img.shields.io/badge/Hysteria2-4ADE80) ![SOCKS5](https://img.shields.io/badge/SOCKS5-4ADE80)

Ссылки `vless://`, `vmess://`, `trojan://`, `ss://`, `hysteria2://`, подписки с заголовками провайдера и полные JSON-конфиги Xray.

## Возможности

| | Windows | macOS | Android | iOS |
|---|:---:|:---:|:---:|:---:|
| **Подписки**: добавление по ссылке, коду или через `ryse://`, автообновление по интервалу провайдера | ✅ | ✅ | ✅ | 🔧 |
| **Автоматический выбор сервера**: пинг всех локаций, карта мира, ручной выбор страны | ✅ | ✅ | ✅ | 🔧 |
| **Режимы работы**: системный прокси или TUN для всего трафика | ✅ | ✅ | системный VPN | 🔧 |
| **Раздельный доступ**: отдельные приложения через VPN или напрямую | ✅ | ✅ | ✅ | 🔧 |
| **Kill switch**: трафик блокируется, если туннель упал | ✅ | 🔧 | — | 🔧 |
| **Переподключение** при смене сети и после сна, с проверкой туннеля | ✅ | ✅ | ✅ | 🔧 |
| **DNS по зашифрованному каналу** и маршрутизация по правилам и геобазам | ✅ | ✅ | ✅ | 🔧 |
| **Уведомления** об окончании подписки, трафик и срок в карточке подписки | ✅ | ✅ | ✅ | 🔧 |
| **Автозапуск и трей**: подключение и отключение без открытия окна | ✅ | ✅ | — | — |
| **Обновления из приложения** с проверкой контрольной суммы | ✅ | ✅ | ✅ | — |
| **Диагностика**: журнал, отчёт без секретов, отправка провайдеру по ссылке | ✅ | ✅ | ✅ | 🔧 |
| **Интерфейс** на русском и английском | ✅ | ✅ | ✅ | 🔧 |

✅ готово · 🔧 в разработке

## Конфиденциальность

Ryse не собирает трафик, ключи и адреса подписок: всё хранится только на вашем устройстве.
Раз в сутки приложение отправляет анонимный сигнал: домен подписки, хеш идентификатора устройства,
система и версия приложения. Его видит только провайдер, подтвердивший свой домен. Отключается в Настройки → Подписки.

## Правовая информация

Ryse не предоставляет VPN-серверы и не продаёт подписки: приложение работает с подпиской вашего провайдера.
Используя приложение, вы соблюдаете законы своей страны.

## Лицензии

Список открытых компонентов (Xray-core, туннели, драйвер, геобазы, флаги, пакеты Flutter) и их лицензий: [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md). В приложении: Настройки → О приложении → «Лицензии».
