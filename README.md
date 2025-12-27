# полезные инструменты для обхода блокировок в России

- https://github.com/igareck/vpn-configs-for-russia - рабочие конфиги vless

- https://github.com/amnezia-vpn/amnezia-client - клиент AmneziaVPN, можно использовать свои конфиги с разными протоколами

- https://github.com/Epodonios/v2ray-configs - конфиги vless, большинство уже скорее всего не будут работать в России, но всё равно полезно

- https://github.com/ImMALWARE/dns.malw.link - обход блокировок со стороны владельцев сайтов с помощью SNI прокси сервера от создателя проекта (gemini или spotify к примеру, https://info.dns.malw.link - сайт)

- https://github.com/bol-van/zapret - утилита для обхода DPI, сложна в настройке для новичка, нужно читать документацию

- https://github.com/bol-van/zapret2 - возможный приемник оригинального zapret (not production ready)

- https://github.com/Flowseal/zapret-discord-youtube - простой обход DPI с готовыми стратегиями (создан на основе zapret от bol-van, подходит только для windows)

- https://github.com/kartavkun/zapret-discord-youtube - простая установка zapret для линукса со стратегиями обхода от flowseal

- https://github.com/nellimonix/warp-config-generator-vercel - генерация конфигов WARP на протоколе AmneziaWG, конфиги подходят только для AmneziaVPN и AmneziaWG (https://warp.llimonix.dev - сайт, https://t.me/warp_generator_bot - телеграмм бот)

- https://github.com/ImMALWARE/bash-warp-generator - создание конфигов WARP для AmneziaVPN/AmneziaWG на удалённом сервере (не совсем user-friendly решение по сравнению с llimonix)

- https://www.torproject.org - в представлении не нуждается, к сожалению заблокировано в России, поэтому для доступа нужно использовать в комбинации с zapret (или другой программой для обхода DPI, в том числе и VPN), в самом браузере tor нужны будут мосты (https://t.me/GetBridgesBot - тг бот, https://bridges.torproject.org/options - сайт, webtunnel мосты более предпочтительны нежели obfs4), есть сторонние варианты использования tor без браузера, но про них я мало знаю

- https://protontestguide.github.io/ProtonVPN-Converter - конвертер конфигов protonvpn из wireguard в amneziawg (требуется иметь аккаунт в proton и создать бесплатный конфиг на сайте по протоколу wireguard, на сам сайт proton можно зайти только с VPN или zapret, https://protonvpn.com - сайт протон)

- https://generator-warp-config.vercel.app - аналог https://warp.llimonix.dev


# советы для безопасности/анонимности

- используйте DoT/DoH (dns over https и dns over tls) на уровне системы или хотя-бы браузера, это позволит избежать утечек DNS, в качестве резолвера советую использовать cloudflare (https://developers.cloudflare.com/1.1.1.1/encryption - больше информации)

- **не** используйте DNS резолвера, который выдаётся вашим провайдером по умолчанию, поменяйте его не проверенного по типу cloudflare, quad9 и т.д.

- (для линуксоидов) к сожалению я не знаю как на windows можно управлять/включить DNSSEC, но на линуксе советую использовать DNSSEC для лучшей безопасности (https://wiki.archlinux.org/title/Systemd-resolved#DNSSEC - включение DNSSEC в линуксе на примере systemd-resolved)

- используйте **всегда** только HTTPS в браузерах (HTTPS-only)

- сохраните нужные файлы/данные для обхода блокировок локально для экстренных случаев

- **не** используйте государственные сервисы/приложения, они собирают данных больше, чем гугл должен российскому суду, не говоря про то, что данные пользователей они хранят в не зашифрованном виде для "собственного удобства"

- это необязательно, но могу посоветовать использовать браузеры librewolf (форк firefox) и brave (основан на chromium), librewolf требует настройки для повседневного использования, в brave измените поисковик с яндекса на любой другой **не** российский

- из расширений для браузеров могу посоветовать uBlock Origin (Lite - если на chromium подобном браузере) и Privacy Badger, в brave эти расширения не нужны

- это необязательно, но мы живём в такое время, что возможно через VPN интернет безопаснее посещать, чем без него, поэтому VPN вам в руки :)

- возможно стоит задуматься над покупкой зарубежного VPS на случай полного пиздеца, чтобы можно было поднять свой VPN/прокси/VLESS сервер

- если вы озабочены уровнем приватности на windows (как я к примеру), то советую хотя-бы ознакомиться с такими линукс дистрибутивами, как linux mint или fedora kde, могу так-же посоветовать Zorin OS, но я меньше с ней ознакомлен и поэтому не ручаюсь за неё
