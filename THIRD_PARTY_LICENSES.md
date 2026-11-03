# Сторонние компоненты и лицензии

RS Connect использует открытые компоненты. Ниже перечислено, что входит в сборки приложения,
под какой лицензией и где взять исходники и полный текст лицензии. Тот же список с полными
текстами открывается в приложении: Настройки → О приложении → «Лицензии».

## Встроенные программы и данные

| Компонент | Назначение | Платформы | Лицензия | Исходники |
|---|---|---|---|---|
| Xray-core | ядро протоколов VLESS, VMess, Trojan, Shadowsocks, REALITY, XHTTP, Hysteria | все | MPL‑2.0 | https://github.com/XTLS/Xray-core |
| hev-socks5-tunnel | туннель TUN → SOCKS5 | Android | MIT | https://github.com/heiher/hev-socks5-tunnel |
| tun2socks | туннель TUN → SOCKS5 | Windows, macOS | MIT | https://github.com/xjasonlyu/tun2socks |
| Wintun | драйвер виртуального сетевого адаптера | Windows | Prebuilt Binaries License | https://www.wintun.net |
| v2ray-rules-dat | геобазы geoip.dat и geosite.dat для правил маршрутизации | все | GPL‑3.0 (данные) | https://github.com/Loyalsoldier/v2ray-rules-dat |
| circle-flags | круглые флаги стран | все | MIT | https://github.com/HatScripts/circle-flags |

Ядро, туннели и драйвер поставляются в виде неизменённых сборок из официальных релизов и работают
как отдельные процессы или системные компоненты. Их исходный код мы не меняем; версии видны в
«О приложении».

## Flutter и пакеты Dart

Приложение написано на Flutter (BSD‑3‑Clause, https://github.com/flutter/flutter). Пакеты из pub.dev
и их лицензии (BSD, MIT, Apache‑2.0) перечислены на странице «Лицензии» в приложении: список
собирается автоматически из самих пакетов при сборке.

## Android

Сборка для Android использует библиотеки AndroidX и Kotlin (Apache‑2.0,
https://github.com/androidx/androidx/blob/androidx-main/LICENSE.txt,
https://github.com/JetBrains/kotlin/blob/master/license/LICENSE.txt).

## Что требуют лицензии

* **MPL‑2.0 (Xray-core)**: текст лицензии прилагается, исходники по ссылке выше; код ядра не изменён.
* **MIT, BSD (туннели, флаги, Flutter, пакеты)**: сохранены уведомления об авторских правах и тексты лицензий.
* **GPL‑3.0 (геобазы)**: файлы данных поставляются без изменений, исходники и текст лицензии по ссылке.
* **Wintun**: драйвер распространяется на условиях лицензии на готовые сборки, текст в приложении.

## Полные тексты

* MPL‑2.0: https://www.mozilla.org/MPL/2.0/
* MIT: https://opensource.org/licenses/MIT
* BSD‑3‑Clause: https://opensource.org/licenses/BSD-3-Clause
* Apache‑2.0: https://www.apache.org/licenses/LICENSE-2.0
* GPL‑3.0: https://www.gnu.org/licenses/gpl-3.0.html
* Wintun Prebuilt Binaries License: https://git.zx2c4.com/wintun/plain/prebuilt-binaries-license.txt

Сам RS Connect — проприетарное приложение; открытые компоненты остаются под своими лицензиями.
