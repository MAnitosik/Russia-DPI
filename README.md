### полезные инструменты для обхода блокировок в России

- **[igareck/vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia)** - рабочие конфиги **vless**, используйте такие клиенты, как **[v2rayNG](https://github.com/2dust/v2rayNG)**, **[v2rayN](https://github.com/2dust/v2rayN)** или **[v2rayA](https://github.com/v2rayA/v2rayA)**

- **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** - клиент **AmneziaVPN**, можно использовать свои конфиги с разными протоколами

- **[Epodonios/v2ray-configs](https://github.com/Epodonios/v2ray-configs)** - конфиги **vless**, далеко не все из них работают, используйте **[v2rayNG](https://github.com/2dust/v2rayNG)**, **[v2rayN](https://github.com/2dust/v2rayN)** или **[v2rayA](https://github.com/v2rayA/v2rayA)**

- **[dns.malw.link](https://github.com/ImMALWARE/dns.malw.link)** - обход блокировок со стороны владельцев сайтов с помощью SNI прокси сервера от создателя проекта (gemini или spotify к примеру, **[сайт](https://info.dns.malw.link)**)

- **[zapret](https://github.com/bol-van/zapret)** - обход DPI, сложна в настройке для новичков, нужно читать документацию, более не получает новых возможностей в пользу **[zapret2](https://github.com/bol-van/zapret2)** (**[zapret](https://github.com/bol-van/zapret)** от **bol-van** это не то же самое, что и **[zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube)** от **Flowseal**)

- **[zapret2](https://github.com/bol-van/zapret2)** - новая версия **[zapret](https://github.com/bol-van/zapret)**, где используется **Lua** для создания стратегий обходов (в теории может быть ещё сложнее, чем классический **[zapret](https://github.com/bol-van/zapret)**, но окупается своей гибкостью с помощью **Lua**)

- **[zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube)** - простой обход DPI с готовыми стратегиями от **Flowseal** для Windows (создан на основе **[zapret](https://github.com/bol-van/zapret)** от **bol-van**, включает в себя файл hosts для Discord с )

- **[kartavkun/zapret-discord-youtube](https://github.com/kartavkun/zapret-discord-youtube)** - простая установка **[zapret](https://github.com/bol-van/zapret)** для линукса со стратегиями обхода от **Flowseal** (**Flowseal** лично **не** причастен к этому проекту)

- **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)** - генерация конфигов **WARP** от cloudflare на протоколе **AmneziaWG**, конфиги подходят только для **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** (**[сайт](https://warp.llimonix.dev)**, **[тг бот](https://t.me/warp_generator_bot)**)

- **[Bash WARP generator](https://github.com/ImMALWARE/bash-warp-generator)** - создание конфигов **WARP** на протоколе **AmneziaWG** для **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** на удалённом сервере (вся инструкция находится в репозитории, не совсем user-friendly решение по сравнению с **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)**)

- **[Tor](https://www.torproject.org)** - в представлении не нуждается, к сожалению не работает из коробки в России, поэтому для доступа нужно использовать в комбинации с другими способами обхода блокировок, в самом браузере **[Tor](https://www.torproject.org)** нужны будут мосты (**[тг бот](https://t.me/GetBridgesBot)**, **[сайт](https://bridges.torproject.org/options)**, **WebTunnel** мосты более предпочтительны)

- **[ProtonVPN converter](https://proton-converter.github.io/proton)** - конвертер конфигов **[Proton VPN](https://protonvpn.com)** из **WireGuard** в **AmneziaWG** для **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** (требуется иметь аккаунт в **[Proton](https://protonvpn.com)** и создать бесплатный конфиг на сайте по протоколу **WireGuard**, на сам сайт **[Proton](https://protonvpn.com)** можно зайти только с помощью утилит для обхода блокировок)

- **[WARP config generator](https://generator-warp-config.vercel.app)** - не хочу особо расписывать, это просто аналог **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)**

- **[v2rayA](https://github.com/v2rayA/v2rayA)** - веб интерфейс для **v2ray**, может быть сложен в установке для новичков, сам интерфейс и его настройка довльно простые (доступ к интерфейсу можно получить по адресу `localhost:2017`)

- **[v2rayN](https://github.com/2dust/v2rayN)** - самый популярный клиент для **v2ray**, особо нечего сказать

- **[v2rayNG](https://github.com/2dust/v2rayNG)** - **[v2rayN](https://github.com/2dust/v2rayN)** для телефонов по сути, создано одним и тем-же человеком

### что использую я

Раньше у меня был провайдер Ростелеком, где на удивление всё легко обходилось. Я переехал и сменил провайдера на местного НН, где блокируется сильно жёстче, чем у Ростелекома по какой то причине (хотя казалось бы Ростелеком самый популярный поставщик интернета в России)

Теперь перейду к нынешнему времени:

Моя ОС - arch linux (btw, да, знаю, очень смешно)

В качестве DNS резолвера использую cloudflare с **DoT** и **DNSSEC** (на удивление cloudflare +- работает без перебоев на моём провайдере)

До недавнего времени использовал этот **[проект](https://github.com/kartavkun/zapret-discord-youtube)**, но даже с ним не всё работало и приходилось комбинировать с **VPN**, на данный момент это мне уже не помогает, а собственные стратегии из **[blockcheck2](https://github.com/bol-van/zapret2/blob/master/docs/manual.md#blockcheck2)** и **[blockcheck](https://github.com/bol-van/zapret/blob/master/docs/quick_start.md#настройка)** для **[zapret2](https://github.com/bol-van/zapret2)** и **[zapret](https://github.com/bol-van/zapret)** соответственно помогают лишь частично

В итоге полностью перешёл на **VPN/v2ray** на данный момент

Итоговый список выглядит так:
1. **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** с конфигами **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)** на **AmneziaWG 1.5** и **[Proton VPN](https://protonvpn.com)** на **AmneziaWG 1.5** (используя **[конвертер](https://proton-converter.github.io/proton/)**)
2. **[v2rayA](https://github.com/v2rayA/v2rayA)** с конфигами **[igareck/vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia)** (в основном сижу на **VPN** ещё, время от времени проверяю работу конфигов **vless**)
3. **[zapret2](https://github.com/bol-van/zapret2)** со стратегиями из **[blockcheck2](https://github.com/bol-van/zapret2/blob/master/docs/manual.md#blockcheck2)** (работает только частично)
4. **[Tor](https://www.torproject.org)** (просто держу у себя, как один из вариантов)

На телефоне использую **[v2rayNG](https://github.com/2dust/v2rayNG)** с теми же конфигами, что и в **[v2rayA](https://github.com/v2rayA/v2rayA)**

### советы для безопасности/анонимности

- используйте **DoT/DoH** (**DNS over HTTPS** или **DNS over TLS**) на уровне системы или хотя бы браузера, это позволит избежать утечек DNS, в качестве резолвера советую использовать cloudflare (**[больше информации](https://developers.cloudflare.com/1.1.1.1/encryption)**)

- **не** используйте DNS резолвера, который выдаётся вашим провайдером по умолчанию, поменяйте его на проверенного по типу cloudflare, quad9 и т.д.

- **Для линукса:** к сожалению я не знаю как на Windows можно управлять/включить **DNSSEC**, но на линуксе советую использовать **DNSSEC** для лучшей безопасности (**[archlinux wiki](https://wiki.archlinux.org/title/Systemd-resolved#DNSSEC)** - включение **DNSSEC** в линуксе на примере systemd-resolved, проверьте поддерживает ли ваш резолвер **DNSSEC**)

- используйте **всегда** только **HTTPS** в браузерах

- сохраните нужные файлы/данные для обхода блокировок локально для экстренных случаев

- **не** используйте государственные сервисы/приложения

- это необязательно, но мы живём в такое время, что возможно через **VPN/прокси** интернет безопаснее посещать, чем без него, поэтому **VPN** вам в руки

- возможно стоит задуматься над покупкой зарубежного VPS на экстренный случай, чтобы можно было поднять свой **VPN/прокси** сервер

### различные сервисы (будет больше в будущем)

- **[LibreSpeed](https://librespeed.org)** - удобный способ проверки скорости интернета с возможностью выбора различных серверов

- **[Cloudflare Speed Test](https://speed.cloudflare.com)** - тест скорости интернета на серверах Cloudflare

- **[Waterfox](https://www.waterfox.com)** - браузер основанный на firefox/gecko, его уникальной особенностью является встроенный **DoOH** (DNS over Oblivious HTTP), что лучше в плане безопасности/анонимности по сравнению с **DoH** или **DoT** (**[больше информации](https://support.mozilla.org/en-US/kb/ohttp-explained)**)

- **[Startpage](https://www.startpage.com)** - поисковик с возможностью открыть любой сайт анонимно через их **прокси** сервера в любом браузере (что к слову обходит блокировки РКН, но помните, что данные с сайта, который вы открываете через их **прокси**, не будут сохранены)

- **[DNSCrypt-proxy](https://github.com/DNSCrypt/dnscrypt-proxy)** - DNS **прокси**, который поддерживает разные безопасные DNS протоколы, может быть сложен для новичков

- **[uBlock Origin](https://github.com/gorhill/uBlock)** - универсальное расширение для браузеров, которое позволяет эффективно блокировать различные элементы в том числе различные трекеры, рекламу, мусор и вирусы
