# URLhaus Malicious URL Blocklist

A blocklist of malicious URLs that are being used for malware distribution, based on the **Database dump (CSV)** of Abuse.ch [URLhaus](https://urlhaus.abuse.ch/).

There are multiple formats available, refer to the appropriate section according to the program used:

- uBlock Origin (uBO) -> [URL-based](#url-based) section (recommended)
- Pi-hole -> [Domain-based](#domain-based) or [Hosts-based](#hosts-based) section
- Hosts file -> [Hosts-based](#hosts-based) section
- Dnsmasq DNS server -> [Dnsmasq](#dnsmasq) section

Not sure which format to choose? See [Compatibility](https://gitlab.com/curben/urlhaus-filter/wikis/compatibility) page in the wiki.

## URL-based

Filter is updated twice a day.

Import the following URL into uBO to subscribe:

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter.txt

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter.txt
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter.txt
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter.txt
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter.txt
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter.txt
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter.txt
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter.txt

</details>

<br />
Lite version (online urls only):

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-online.txt

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-online.txt
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-online.txt
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-online.txt
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-online.txt
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-online.txt
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-online.txt
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-online.txt

</details>

**Note:** Lite version is ~95% smaller by excluding offline urls. The status of urls is determined by the upstream Abuse.ch. However, the test is not 100% accurate and some malicious urls that are otherwise accessible may be missed. If bandwidth (1.5MB/day) is not a constraint, I recommend the regular version.

*PS: While regular version contains roughly 65K filters, uBO can [easily handle](https://github.com/uBlockOrigin/uBlock-issues/issues/338#issuecomment-452843669) half a million filters.*

## Domain-based

This blocklist includes domains and IP addresses.

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-domains.txt

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-domains.txt
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-domains.txt
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-domains.txt
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-domains.txt
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-domains.txt
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-domains.txt
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-domains.txt

</details>

<br />
Lite version (online domains/IPs only):

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-domains-online.txt

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-domains-online.txt
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-domains-online.txt
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-domains-online.txt
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-domains-online.txt
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-domains-online.txt
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-domains-online.txt
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-domains-online.txt

</details>

## Hosts-based

This blocklist includes domains only.

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts.txt

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts.txt
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts.txt
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-hosts.txt
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-hosts.txt
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-hosts.txt
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-hosts.txt
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-hosts.txt

</details>

<br />
Lite version (online domains only):

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts-online.txt

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts-online.txt
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-hosts-online.txt
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-hosts-online.txt
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-hosts-online.txt
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-hosts-online.txt
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-hosts-online.txt
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-hosts-online.txt

</details>

## Dnsmasq

This blocklist includes domains only.

### Install

```
mkdir -p ~/.config/urlhaus-filter/
curl https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq.conf -o ~/.config/urlhaus-filter/urlhaus-filter-dnsmasq.conf
printf "\nconf-file=$HOME/.config/urlhaus-filter/urlhaus-filter-dnsmasq.conf\n" >> /etc/dnsmasq.conf
```

### Update

```
curl https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq.conf -o ~/.config/urlhaus-filter/urlhaus-filter-dnsmasq.conf
```

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq.conf
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq.conf
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-dnsmasq.conf
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-dnsmasq.conf
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-dnsmasq.conf
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-dnsmasq.conf
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-dnsmasq.conf

</details>

<br />
Lite version (online domains only):

- https://gitlab.com/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq-online.conf

<details>
<summary>Mirrors</summary>

- https://cdn.statically.io/gl/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq-online.conf
- https://glcdn.githack.com/curben/urlhaus-filter/raw/master/urlhaus-filter-dnsmasq-online.conf
- https://raw.githubusercontent.com/curbengh/urlhaus-filter/master/urlhaus-filter-dnsmasq-online.conf
- https://cdn.statically.io/gh/curbengh/urlhaus-filter/master/urlhaus-filter-dnsmasq-online.conf
- https://gitcdn.xyz/repo/curbengh/urlhaus-filter/master/urlhaus-filter-dnsmasq-online.conf
- https://cdn.jsdelivr.net/gh/curbengh/urlhaus-filter/urlhaus-filter-dnsmasq-online.conf
- https://repo.or.cz/urlhaus-filter.git/blob_plain/refs/heads/master:/urlhaus-filter-dnsmasq-online.conf

</details>

Note that it is not possible for Dnsmasq to block malicious IP address.

## Issues

Report any false positive by creating an [issue](https://gitlab.com/curben/urlhaus-filter/issues) or [merge request](https://gitlab.com/curben/urlhaus-filter/merge_requests)

This filter **only** accepts malware URLs from [URLhaus](https://urlhaus.abuse.ch/).

Please report new malware URL to the upstream maintainer through https://urlhaus.abuse.ch/api/#submit.

This repo is not endorsed by Abuse.ch.

## Cloning

Since the filter is updated frequently, cloning the repo would become slower over time as the revision grows.

Use shallow clone to get the recent revisions only. Getting the last five revisions should be sufficient for a valid MR.

`git clone --depth 5 https://gitlab.com/curben/urlhaus-filter.git`

## License

[Creative Commons Zero v1.0 Universal](LICENSE.md)

## FAQ

See [FAQ](https://gitlab.com/curben/urlhaus-filter/wikis/faq).
