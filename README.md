# shadowsocks-libev
Shadowsocks-libev is a lightweight secured SOCKS5 proxy for embedded devices and low-end boxes.

It is a port of Shadowsocks created by @clowwindy, which is maintained by @madeye and @linusyang.

Shadowsocks-libev is written in pure C and only depends on libev and OpenSSL or mbedTLS or PolarSSL.

In normal usage, the memory footprint is about 600KB and the CPU utilization is no more than 5% on a low-end router (Buffalo WHR-G300N V2 with a 400MHz MIPS CPU, 32MB memory and 4MB flash).

## Dependencies

* libev (*libevent instead*, it's offical support.)
* OpenSSL (Offical support)

## Build

```sh
source shadowsocks-libev.info
wget $DOWNLOAD
sudo sh shadowsocks-libev.SlackBuild
# slackware
sudo installpkg /tmp/shadowsocks-libev-2.5.3-i?86-1_SBo.tgz
# slackware64
sudo installpkg /tmp/shadowsocks-libev-2.5.3-x86_64-1_SBo.tgz
```