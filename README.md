### полезные инструменты для обхода блокировок в России

- **[igareck/vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia)** - рабочие конфиги **VLESS**, используйте такие клиенты, как **[v2rayNG](https://github.com/2dust/v2rayNG)**, **[v2rayN](https://github.com/2dust/v2rayN)** или **[v2rayA](https://github.com/v2rayA/v2rayA)**

- **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** - клиент **AmneziaVPN**, можно использовать свои конфиги с разными протоколами

- **[Epodonios/v2ray-configs](https://github.com/Epodonios/v2ray-configs)** - конфиги **VLESS**, далеко не все из них работают, используйте **[v2rayNG](https://github.com/2dust/v2rayNG)**, **[v2rayN](https://github.com/2dust/v2rayN)** или **[v2rayA](https://github.com/v2rayA/v2rayA)**

- **[dns.malw.link](https://github.com/ImMALWARE/dns.malw.link)** - обход блокировок со стороны владельцев сайтов с помощью SNI прокси сервера от создателя проекта (gemini или spotify к примеру, **[сайт](https://info.dns.malw.link)**)

- **[zapret](https://github.com/bol-van/zapret)** - утилита для обхода DPI, сложна в настройке для новичка, нужно читать документацию (не тот, который от **flowseal**)

- **[zapret2](https://github.com/bol-van/zapret2)** - более лучшая версия **[zapret](https://github.com/bol-van/zapret)**, где используется **Lua** для создания стратегий обходов (сложнее, чем классический **[zapret](https://github.com/bol-van/zapret)**)

- **[zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube)** - простой обход DPI с готовыми стратегиями от **flowseal** (создан на основе **[zapret](https://github.com/bol-van/zapret)** от **bol-van**, подходит только для windows, с недавнего времени включает в себя файл hosts для дискорда в обход DNS запросам)

- **[kartavkun/zapret-discord-youtube](https://github.com/kartavkun/zapret-discord-youtube)** - простая установка **[zapret](https://github.com/bol-van/zapret)** для линукса со стратегиями обхода от **flowseal** (**flowseal** лично **не** причастен к этому проекту)

- **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)** - генерация конфигов **WARP** от cloudflare на протоколе **AmneziaWG**, конфиги подходят только для **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** (**[сайт](https://warp.llimonix.dev)**, **[тг бот](https://t.me/warp_generator_bot)**)

- **[Bash WARP generator](https://github.com/ImMALWARE/bash-warp-generator)** - создание конфигов **WARP** на протоколе **AmneziaWG** для **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** на удалённом сервере (вся инструкция находится в репозитории, не совсем user-friendly решение по сравнению с **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)**)

- **[Tor](https://www.torproject.org)** - в представлении не нуждается, к сожалению не работает из коробки в России, поэтому для доступа нужно использовать в комбинации с другими способами обхода блокировок, в самом браузере **[Tor](https://www.torproject.org)** нужны будут мосты (**[тг бот](https://t.me/GetBridgesBot)**, **[сайт](https://bridges.torproject.org/options)**, **webtunnel** мосты более предпочтительны)

- **[ProtonVPN converter](https://proton-converter.github.io/proton)** - конвертер конфигов **[Proton VPN](https://protonvpn.com)** из **wireguard** в **AmneziaWG** для **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** (требуется иметь аккаунт в **[Proton](https://protonvpn.com)** и создать бесплатный конфиг на сайте по протоколу **wireguard**, на сам сайт **[Proton](https://protonvpn.com)** можно зайти только с помощью утилит для обхода блокировок)

- **[WARP config generator](https://generator-warp-config.vercel.app)** - не хочу особо расписывать, это просто аналог **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)**

- **[v2rayA](https://github.com/v2rayA/v2rayA)** - веб интерфейс для **v2ray**, может быть сложен в установке для новичков, сам интерфейс и его настройка довльно простые (доступ к интерфейсу можно получить по адресу "localhost:2017")

- **[v2rayN](https://github.com/2dust/v2rayN)** - самый популярный клиент для **v2ray**, особо нечего сказать

- **[v2rayNG](https://github.com/2dust/v2rayNG)** - **[v2rayN](https://github.com/2dust/v2rayN)** для телефонов по сути, создано одним и тем-же человеком

### что используя я
Раньше у меня был провайдер ростелеком, где на удивление всё легко обходилось. Я переехал и сменил провайдера на местного НН, где блокируется сильно жёстче, чем у ростелекома по какой-то причине (хотя казалось бы ростелеком наиболее всего приближён к государству)

Теперь перейду к нынешнему времени:

Моя ОС - arch linux (btw, да, знаю, очень смешно)

В качестве DNS резолвера использую cloudflare с **DoT** и **DNSSEC** (на удивление cloudflare +- работает без перебоев на моём провайдере)

До недавнего времени использовал этот **[проект](https://github.com/kartavkun/zapret-discord-youtube)**, но даже с ним не всё работало и приходилось комбинировать с **VPN**, на данный момент **[zapret](https://github.com/bol-van/zapret)** сам по себе начал плохо работать у меня, и в целом интернет с ним помирал (даже на сайтах, которые не заблокированы)

В итоге полностью перешёл на **VPN** на данный момент

Итоговый список выглядит так:
1. **[AmneziaVPN](https://github.com/amnezia-vpn/amnezia-client)** с конфигами **[WARP llimonix](https://github.com/nellimonix/warp-config-generator-vercel)** на **AmneziaWG 1.5** и **[Proton VPN](https://protonvpn.com)** на **AmneziaWG 1.5** (используя **[конвертер](https://proton-converter.github.io/proton/)**)
2. **[v2rayA](https://github.com/v2rayA/v2rayA)** с конфигами **[igareck/vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia)** и **[Epodonios/v2ray-configs](https://github.com/Epodonios/v2ray-configs)** (в основном сижу на **VPN** ещё, время от времени проверяю работу конфигов **VLESS**)
3. **[zapret2](https://github.com/bol-van/zapret2)** со стратегиями из **[blockcheck2](https://github.com/bol-van/zapret2/blob/master/docs/manual.md#blockcheck2)** (ещё тестирую, пока что нечего сказать)
4. **[Tor](https://www.torproject.org)** (держу у себя на всякий случай, не бывает лишним)

На телефоне использую **[v2rayNG](https://github.com/2dust/v2rayNG)** с теми же конфигами, что и в **[v2rayA](https://github.com/v2rayA/v2rayA)**

### советы для безопасности/анонимности

- используйте **DoT/DoH** (**dns over https** и **dns over tls**) на уровне системы или хотя-бы браузера, это позволит избежать утечек DNS, в качестве резолвера советую использовать cloudflare (**[больше информации](https://developers.cloudflare.com/1.1.1.1/encryption)**)

- **не** используйте DNS резолвера, который выдаётся вашим провайдером по умолчанию, поменяйте его на проверенного по типу cloudflare, quad9 и т.д.

- (для линуксоидов) к сожалению я не знаю как на windows можно управлять/включить **DNSSEC**, но на линуксе советую использовать **DNSSEC** для лучшей безопасности (**[archlinux wiki](https://wiki.archlinux.org/title/Systemd-resolved#DNSSEC)** - включение **DNSSEC** в линуксе на примере systemd-resolved, проверьте поддерживает ли ваш резолвер **DNSSEC**)

- используйте **всегда** только **HTTPS** в браузерах (**HTTPS-Only**)

- сохраните нужные файлы/данные для обхода блокировок локально для экстренных случаев

- **не** используйте государственные сервисы/приложения, они собирают данных больше, чем гугл должен российскому суду, не говоря про то, что данные пользователей они хранят в не зашифрованном виде для "собственного удобства"

- это необязательно, но мы живём в такое время, что возможно через **VPN** интернет безопаснее посещать, чем без него, поэтому **VPN** вам в руки :)

- возможно стоит задуматься над покупкой зарубежного VPS на случай полного пиздеца, чтобы можно было поднять свой **VPN/прокси** сервер
