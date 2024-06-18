# adguard-extension-settings

My recommendations for the ultimate configuration of AdGuard's browser extension :)

**NOTE:** For AdGuard on Safari on iOS, see [here](https://codeberg.org/Magnesium1062/adguard-safari-settings-ios), and for AdGuard on Safari on macOS, see [here](https://codeberg.org/Magnesium1062/adguard-safari-settings-macos).

# General

**Block search ads and websites' self-promotion** -> ✅

**Phishing and malware protection** -> ❌ *(Use [Quad9](https://www.quad9.net/) instead)*

**Activate the most appropiate filters automatically** -> ✅

**Auto-update filters** -> `1 hour` *(If this causes you any issues, you can set to `6 hours` instead)*

# Filters

I would generally recommend enabling most of the built-in filters, besides those under the `Language-specific` category & some of those under the `Other` category. These are all extremely carefully picked lists with strong coverage and minimal breakage, and I would recommend enabling them as follows for the best coverage possible.

**Ad Blocking** -> ✅

Ad Blocking:

* `AdGuard Base filter` -> ✅

* `AdGuard Mobile Ads filter` -> ✅

* `EasyList` -> ✅


**Privacy** -> ✅

Privacy:

* `AdGuard Tracking Protection filter` -> ✅

* `AdGuard URL Tracking filter` -> ✅

* `EasyPrivacy` -> ✅

* `Legitimate URL Shortener` -> ✅

* `Peter Lowe's Blocklist` -> ✅

* `Fanboy's Anti-Facebook List` -> ✅


**Social Widgets** -> ✅

Social Widgets:

* `AdGuard Social Media filter` -> ✅

* `Fanboy's Social Blocking List` -> ✅


**Annoyances** -> ✅

Annoyances:

`AdGuard Cookie Notices filter` -> ✅

`AdGuard Popups filter` -> ✅

`AdGuard Mobile App Banners filter` -> ✅

`AdGuard Other Annoyances filter` -> ✅

`AdGuard Widgets filter` -> ✅

`AdGuard Annoyances filter` -> ✅

`Adblock Warning Removal List` -> ✅

`Fanboy's Annoyances` -> ✅

`EasyList Cookie List` -> ✅

`Dandelion Sprout's Annoyances List` -> ✅

**Security** -> ✅

Security:

`Online Malicious URL Blocklist` -> ✅

`Phishing URL Blocklist` -> ✅

`Scam Blocklist by DurableNapkin` -> ✅ *(Only enable this if you don't also have DNS content blocking with this list enabled in place, otherwise keep this list disabled)*

`uBlock Origin - Badware risks` -> ✅

**Other** -> ✅

Other:

`AdGuard DNS filter` -> ✅  *(Only enable this if you don't also have DNS content blocking with this list enabled in place, otherwise keep this list disabled and re-disable the `Other` category)*

**Custom** -> ✅

Custom:

I would recommend importing the following lists:

* ⭐️ `Divested - Fingerprinting` - `https://codeberg.org/divested/dnsbl/raw/branch/master/Fingerprinting.ubl`

* ⭐️ `HaGeZi's Threat Intelligence Feeds - IPs`: `https://raw.githubusercontent.com/hagezi/dns-blocklists/main/ips/tif.txt` *(Even if you use this list in i.e. AdGuard Home, you should also apply it here for an extra level of protection from these IPs outside of just the DNS level)*

* ⭐️ `pfBlockerNG MS-1`: `https://gist.githubusercontent.com/BBcan177/bf29d47ea04391cb3eb0/raw/7290e0681bcd07415420b5c80a253652fd13f840/MS-1` *(Even if you use this list in i.e. AdGuard Home, you should also apply it here for an extra level of protection from these IPs outside of just the DNS level)*

* ⭐️ Yokoffing's `Block third party fonts`: `https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt`

Additionally, if you don't have a DNS content blocking solution in place *(you should)*, or you just can't use the relevant list on your DNS blocker, you should import the following:

* ⭐️ My `BadBlock`: `https://codeberg.org/Magnesium1062/BadBlock/raw/branch/main/abp/badblock.txt`

* ⭐️ `Dandelion Sprout's Anti-Malware List`: `https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt`

* ⭐️ `Divested Combined Blocklist`: `https://divested.dev/hosts-domains-wildcards`

* ⭐️ `HaGeZi's Badware Host Blocking`: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/hoster.txt`

* ⭐️ `HaGeZi's Most Abused TLDs`: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/spam-tlds-ublock.txt`

* ⭐️ `HaGeZi Multi PRO++`: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/pro.plus.txt`

* ⭐️ `HaGeZi's Threat Intelligence Feeds`: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/tif.txt`

* ⭐️ `HaGeZi/xRuffKez's Newly Registered Domains (14 days)`: `https://raw.githubusercontent.com/xRuffKez/NRD/main/nrd-14day_adblock.txt`

* ⭐️ `OISD - Big`: `https://big.oisd.nl`

Additionally, if you're fine with a little breakage, I would highly recommend:

* ⭐️ My `BadBlock `**+** instead of `BadBlock`: `https://codeberg.org/Magnesium1062/BadBlock/raw/branch/main/abp/badblock_plus.txt`

* ⭐️ `1Hosts Pro`: `https://o0.pages.dev/Pro/adblock.txt`

* ⭐️ `HaGeZi Multi` **Ultimate** instead of `HaGezi Multi` **Pro++**: `https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/ultimate.txt`

# Stealth Mode

**Stealth Mode** -> ✅

General -> **Block trackers** -> ✅

General -> **Remove tracking parameters** -> ✅

General -> **Hide your search queries** -> ✅

General -> **Ask websites not to track you** -> ✅

Cookies -> **Self-destruction of third-party cookies** -> ✅

Cookies -> **Self-destruction of third-party cookies** -> Your choice, the shorter the better, I usually leave at the default of `2880`

Miscellaneous -> **Hide Referrer from third parties** -> ✅

Miscellaneous -> **Disable WebRTC** -> ❌ *(As long as you're using a private browser like Firefox or Brave, then there really isn't a point or benefit from setting this IMO)*

# User rules

**User rules** -> ✅

User rules:

This is where it can really depend on you and your set-up. I'll provide my recommendations and filters here I myself use below:

First, I would highly recommend setting the following to protect against [IDN Homograph attacks](https://wikipedia.org/wiki/IDN_homograph_attack) *You don't need to set this if your DNS provider already provides IDN Homograph Attacks Protection (i.e. NextDNS)*:

`xn--*`

`xn--*$doc,popup,frame`

I usually also set the following to always enforce blocking Google's Doubleclick & Google Analytics: ((Why?)[https://github.com/gorhill/uBlock/wiki/Privacy-stuff])

`||doubleclick.net^$important`

`||google-analytics.com^$important`

Additionally, I set the following to block social media tracking on websites:

`||facebook.com^$important,third-party`

`||facebook.net^$important,third-party`

`||linkedin.com^$important,third-party`

`||instagram.com^$important,third-party`

`||tiktok.com^$important,third-party`

I also set this to block [tracking from Gravatar](https://github.com/gorhill/uBlock/wiki/Privacy-stuff):

`||gravatar.com^$important,third-party`

I also set these rules to block 3rd party sign-in prompts from Google & Apple, as they're 1: annoying and 2: a tracking concern:

`||accounts.google.com^$third-party`

`||appleid.apple.com^$third-party`

`||appleid.cdn-apple.com^$third-party`

`@@||accounts.google.com^$domain=youtube.com|chromium.org|gstatic.com|googleusercontent.com`

`@@||appleid.apple.com^$domain=appleid.cdn-apple.com`

`@@||appleid.cdn-apple.com^$domain=appleid.apple.com`

Finally, I usually set the following to block the annoying banner on Old Reddit promoting Reddit's new UI.

`www.reddit.com###redesign-beta-optin-btn`

`old.reddit.com###redesign-beta-optin-btn`

Once you are done here, make sure to select `Save`.

# Additional settings

**Use optimized filters** -> ❌

**Invert allowlist** -> ❌ *(Should be default)*

**Help with the development of AdGuard filters** -> ❌

**Show information on the AdGuard full version** -> ❌

**Notify about extension updates** -> ✅

# Additional recommendations

* Use a privacy-respecting browser like [Firefox](https://www.mozilla.org/firefox/).

* Enable Safe Browsing in your browser if possible and if it's not done in a privacy-invasive way. (You should use i.e. [Google Safe Browsing on "Standard" Mode](https://safebrowsing.google.com/), [Firefox's Safe Browsing](https://support.mozilla.org/kb/how-does-phishing-and-malware-protection-work), & [Brave's Safe Browsing](https://brave.com/privacy/browser/#safe-browsing), you should avoid most other options i.e. [Google Safe Browsing on "Enhanced" Mode](https://safebrowsing.google.com/), [Microsoft SmartScreen](https://learn.microsoft.com/windows/security/operating-system-security/virus-and-threat-protection/microsoft-defender-smartscreen/), & [Opera Sitecheck](https://blogs.opera.com/security/2021/01/making-browsing-safe-from-phishing/)).

* Use a private, secure, & reputable DNS provider of your choice. I would recommend setting up your own [NextDNS](https://nextdns.io) configuration if you are able to *(See my recommendations for NextDNS [here](https://codeberg.org/Magnesium1062/nextdns-settings))*, otherwise I would recommend [Quad9](https://quad9.net/). *(Even if you have a private/secure DNS provider set on your OS/network level, make sure to also set it in your browser as well, so that you can take advantage of [Encrypted Client Hello](https://blog.cloudflare.com/announcing-encrypted-client-hello))*

* Use a (reputable) anti-virus if possible. On Windows, you can use the built-in [Microsoft Defender Antivirus](https://en.wikipedia.org/wiki/Microsoft_Defender_Antivirus), on macOS, you can stick to the built-in [XProtect](https://support.apple.com/guide/security/protecting-against-malware-sec469d47bd8/web), on Android, you can use [Hypatia](https://f-droid.org/packages/us.spotco.malwarescanner/), and on Linux, you can use [ClamAV](https://www.clamav.net/). **NOTE:** You should install Hypatia through the [DivestOS Official Repo](https://divestos.org/fdroid/official/?fingerprint=E4BE8D6ABFA4D9D4FEEF03CDDA7FF62A73FD64B75566F6DD4E5E577550BE8467) instead of F-Droid's main repo, as it will allow you to receive quicker updates directly from the developer. It's also recommended to use [F-Droid Basic](https://f-droid.org/en/packages/org.fdroid.basic/) as your F-Droid client of choice.