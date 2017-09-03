# shadowsocks-libev
Shadowsocks-libev is a lightweight secured SOCKS5 proxy for embedded devices and low-end boxes.

It is a port of Shadowsocks created by @clowwindy, which is maintained by @madeye and @linusyang.

Shadowsocks-libev is written in pure C and only depends on libev and OpenSSL or mbedTLS or PolarSSL.

In normal usage, the memory footprint is about 600KB and the CPU utilization is no more than 5% on a low-end router (Buffalo WHR-G300N V2 with a 400MHz MIPS CPU, 32MB memory and 4MB flash).

## Dependencies

* libev (*libevent instead*, it's offical support.)
* OpenSSL (Offical support)
* mbedtls
* libsodium
* udns
* pcre3 (or maybe pcre2)
* c-ares

## Build

**NOTE: the source package in upstream's github release page is incomplete. Please issue:**

```sh
git clone --recursive -j8 https://github.com/shadowsocks/shadowsocks-libev.git shadowsocks-libev-3.0.8
tar --remove-fils -cvzf v3.0.8.tar.gz shadowsocks-libev-3.0.8
sudo bash shadowsocks-libev.SlackBuild

# slackware
sudo installpkg /tmp/shadowsocks-libev-2.5.3-i?86-1_SBo.tgz

# slackware64
sudo installpkg /tmp/shadowsocks-libev-2.5.3-x86_64-1_SBo.tgz
```
