> Only for experienced users.

# AdGuardHome DNS Filter List<a name="adguardhome-dns-filter-list"></a> <a href="#"><img src="https://badgen.net/github/last-commit/luckmagnet/adguard-filter-list?label=Updated&cache=0&color=green&icon=github" alt="Last commit activity"></a>

______________________________________________________________________

<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=1 -->

- [AdGuardHome DNS Filter List](#adguardhome-dns-filter-list)
  - [What Is This?](#what-is-this)
  - [How Can I Use It?](#how-can-i-use-it)
  - [Which Lists Are Combined Here?](#which-lists-are-combined-here)
  - [Do You Curate the Lists?](#do-you-curate-the-lists)
  - [How Often Is This List Updated?](#how-often-is-this-list-updated)
  - [Whitelist Exceptions You Might Want to Make](#whitelist-exceptions-you-might-want-to-make)
    - [Google Fonts](#google-fonts)
  - [Last Words](#last-words)

<!-- mdformat-toc end -->

______________________________________________________________________

## What Is This?<a name="what-is-this"></a>

This is a DNS blocklist that can be used for AdGuardHome. 

This list combines more than XX other lists, including most of the default lists from
AdGuardHome, into one single list, so you don't have to add countless lists to your
AdGuardHome, but just this one.

## How Can I Use It?<a name="how-can-i-use-it"></a>

Pretty simple, copy this link
(https://raw.githubusercontent.com/luckmagnet/adguard-filter-list/master/blocklist) and add it to your AdGuardHome DNS blocklists.

> [!TIP]
> If the IP list is used in AdGuard Home, all domains that would resolve to the blocked IP are blocked. To prevent the blocked domains from being resolved via IPv6, it is necessary to deactivate resolving via IPv6 in AdGuard Home:                        
> `Settings > DNS settings > DNS server configuration > Disable resolving of IPv6 addresses`
> 
## Which Lists Are Combined Here?<a name="which-lists-are-combined-here"></a>

Which lists I'm using here, you can see in hostlist compiler configuration
» [click here](hostlist-compiler-config.json) « or have a look at the table below.

| Name                                                                      | URL                                                                                                                                              |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Hagezi's Multi ULTIMATE                                                     | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/ultimate.txt                                                                    |
| Hagezi's Threat Intelligence Feeds                                          | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/tif.txt                                                                         |
| Newly registered entropy domains (entropy NRDs/DGAs)                      | https://raw.githubusercontent.com/hagezi/nrd/main/adblock/dga7.txt                                                                               |
| HaGeZi's Encrypted DNS/VPN/TOR/Proxy Bypass DNS Blocklist                 | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/doh-vpn-proxy-bypass.txt                                                        |
| Encrypted DNS Servers IPs                                                 | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/doh-ips.txt                                                                     |
| HaGeZi's DynDNS Blocklist                                                 | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/dyndns.txt                                                                      |
| HaGeZi's Badware Hoster DNS Blocklist                                     | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/hoster.txt                                                                      |
| HaGeZi's Blocklist URL Shortener                                          | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/urlshortener.txt                                                                |
| HaGeZi's The World's Most Abused TLDs                                     | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/spam-tlds.txt                                                                   |
| HaGeZi's DNS Rebind Protection                                            | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adguard/dns-rebind-protection.txt                                                       |
| Steven Black's Unified hosts                                              | https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts                                                                                 |
| Dandelion Sprout's AdGuard Home Compilation List - Web Push Notifications | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/AdGuard%20Home%20Compilation%20List/AdGuardHomeCompilationList-Notifications.txt |
| Perflyst and Dandelion Sprout's Smart-TV Blocklist                        | https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/SmartTV-AGH.txt                                                                |
| Dandelion Sprout's Game Console Adblock List                              | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/GameConsoleAdblockList.txt                                                       |
| FMHY Unsafe sites filterlist - Plus                                       | https://raw.githubusercontent.com/fmhy/FMHYFilterlist/main/filterlist.txt                                                                        |
| Hagezi's Threat Intelligence Feeds - IPs                                             | https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/tif-ips.txt                                    |
|  Dandelion Sprout's Anti-Malware List                                        | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Alternate%20versions%20Anti-Malware%20List/AntiMalwareAdGuardHome.txt                                                           |
| xRuffKez CTI (Cyber Threat Intelligence)                                                                 | https://raw.githubusercontent.com/DNSBunker/CTI/main/adblock.txt                                                                                     |
| EasyPrivacy                                                       | https://easylist.to/easylist/easyprivacy.txt                                                                                                           |
| uBlock filters - Default                                                  | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/filters.txt                                                                |
| uBlock filters – Badware risks                                            | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/badware.txt                                                                |
| uBlock filters – Privacy                                                  | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/privacy.txt                                                                |
| uBlock filters – Resource abuse                                           | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/resource-abuse.txt                                                         |
| Frellwit's Swedish Filter                                                  | https://raw.githubusercontent.com/lassekongo83/Frellwits-filter-lists/master/Frellwits-Swedish-Filter.txt                                                                |
| OISD Big List                                                             | https://big.oisd.nl                                                                                                                              |
| Phishing URL Blocklist                                          | https://curbengh.github.io/phishing-filter/phishing-filter-agh.txt                                                                    |
| Dandelion Sprouts nordiske filtre                                                  | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/NorwegianExperimentalList%20alternate%20versions/NordicFiltersAdGuardHome.txt                                                                            |
| ShadowWhisperer's Malware List                                                 | https://raw.githubusercontent.com/ShadowWhisperer/BlockLists/master/Lists/Malware                                                                           |
|                                            |                                                                      |
|                                        |                                                                  |
| PolishFiltersTeam - KADhosts                                              | https://raw.githubusercontent.com/PolishFiltersTeam/KADhosts/master/KADhosts.txt                                                                 |
| FadeMind - Hosts Extra (Spam Hosts)                                       | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Spam/hosts                                                                    |
| Firebog - Personal Blocklist by WaLLy3K                                   | https://v.firebog.net/hosts/static/w3kbl.txt                                                                                                     |
| Firebog - Neohostsbasic                                                   | https://v.firebog.net/hosts/neohostsbasic.txt                                                                                                    |
| Firebog - AdGuardDNS                                                      | https://v.firebog.net/hosts/AdguardDNS.txt                                                                                                       |
| Firebog - Admiral                                                         | https://v.firebog.net/hosts/Admiral.txt                                                                                                          |
| Firebog - Easylist                                                        | https://v.firebog.net/hosts/Easylist.txt                                                                                                         |
| Firebog - Prigent Crypto                                                  | https://v.firebog.net/hosts/Prigent-Crypto.txt                                                                                                   |
| Firebog - Prigent Malware                                                 | https://v.firebog.net/hosts/Prigent-Malware.txt                                                                                                  |
| Matomo - Referrer Spam Blacklist                                          | https://raw.githubusercontent.com/matomo-org/referrer-spam-blacklist/master/spammers.txt                                                         |
| Matomo.org - Referrer Spammers                                            | https://raw.githubusercontent.com/matomo-org/referrer-spam-list/master/spammers.txt                                                              |
| VeleSila - yhosts                                                         | https://raw.githubusercontent.com/VeleSila/yhosts/master/hosts                                                                                   |
| RooneyMcNibNug - PiHole Stuff (SNAFU)                                     | https://raw.githubusercontent.com/RooneyMcNibNug/pihole-stuff/master/SNAFU.txt                                                                   |
| anudeepND - Adservers                                                     | https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt                                                                       |
| anudeepND - Facebook                                                      | https://raw.githubusercontent.com/anudeepND/blacklist/master/facebook.txt                                                                        |
| Ad filter list by Disconnect                                              | https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt                                                                                       |
| Peter Lowe's List                                                         | https://pgl.yoyo.org/adservers/serverlist.php?hostformat=adblockplus&showintro=1&mimetype=plaintext                                              |
| Perflyst and Dandelion Sprout's Smart-TV Blocklist                        | https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/SmartTV-AGH.txt                                                                |
| Spam404 - Main Blacklist                                                  | https://raw.githubusercontent.com/Spam404/lists/master/main-blacklist.txt                                                                        |
| Spam404 - Adblock List                                                    | https://raw.githubusercontent.com/Spam404/lists/master/adblock-list.txt                                                                          |
| Game Console Adblock List                                                 | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/GameConsoleAdblockList.txt                                                       |
| NoCoin Filter Lis                                                         | https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/hosts.txt                                                                 |
|                                                            |                                                                                                               |
| FadeMind - UncheckyAds                                                    | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/UncheckyAds/hosts                                                                 |
| FadeMind - Additional Risks                                               | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Risk/hosts                                                                    |
|                                                        |                                                                                  |
| jdlingyu - ad-wars                                                        | https://raw.githubusercontent.com/jdlingyu/ad-wars/master/hosts                                                                                  |
| ethanr - DNS-Blacklists                                                   | https://bitbucket.org/ethanr/dns-blacklists/raw/8575c9f96e5b4a1308f2f12394abd86d0927a4a0/bad_lists/Mandiant_APT1_Report_Appendix_D.txt           |
| NoTrack Malware Blocklist                                                 | https://gitlab.com/quidsup/notrack-blocklists/raw/master/notrack-malware.txt                                                                     |
|                                                 |                                                                                                      |
|                                                        |                                                                                  |
| Adblock Warning Removal List                                              | https://easylist-downloads.adblockplus.org/antiadblockfilters.txt                                                                                |
| ABP filters                                                               | https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt                                                                               |
| AdGuard CNAME disguised trackers list                                     | https://raw.githubusercontent.com/AdguardTeam/cname-trackers/master/data/combined_disguised_trackers.txt                                         |
| Easylist Cookie List                                                      | https://secure.fanboy.co.nz/fanboy-cookiemonster.txt                                                                                             |
|                                                                |                                                                                                      |                                                           |
| Firebog - Easyprivacy                                                     | https://v.firebog.net/hosts/Easyprivacy.txt                                                                                                      |
| Firebog - Prigent-Ads                                                     | https://v.firebog.net/hosts/Prigent-Ads.txt                                                                                                      |
| FadeMind - hosts.extras/add.2o7Net                                        | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.2o7Net/hosts                                                                  |
| Malvertising list by Disconnect                                           | https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt                                                                             |
|                                      |                                                                           |
|                                               |                                                                    |
|                            |                                                     |
|                                                |                                                                     |
|                           |                                                                      |
| FR: French filters RedFlagDomains                                         | https://dl.red.flag.domains/red.flag.domains.txt                                                                                                 |

## Do You Curate the Lists?<a name="do-you-curate-the-lists"></a>

Absolutely not.

All these lists are considered 3rd party from my point of view. I have no influence
over them at all. All I do is combine the lists I was using into one single list, so
my list of blocklists isn't massive. (That was a lot of lists in one sentence ...)

## How Often Is This List Updated?<a name="how-often-is-this-list-updated"></a>

Once a day

## Whitelist Exceptions You Might Want to Make<a name="whitelist-exceptions-you-might-want-to-make"></a>

### Google Fonts<a name="google-fonts"></a>

As stated [here](https://github.com/lightswitch05/hosts#google-fonts) from one of
the lists I am using, you might have to whitelist `fonts.gstatic.com`. To do so, add
the following to your whitelist:

```plainext
@@||fonts.gstatic.com^$important
```

## Last Words<a name="last-words"></a>

You are free to use this list, but I can give you no guarantee for it since none of
the lists combined here is managed by me.

If you want to create your own combined list, feel free to fork this repository and
change the hostlist compiler configuration I included to start your own voyage. To
compile the hostlist, use
[AdGuard's HostlistCompiler](https://github.com/AdguardTeam/HostlistCompiler).
