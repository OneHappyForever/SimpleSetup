# SimpleSetup

Install BBR and secure SSR

BBR Installation:
```
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
chmod +x bbr.sh
./bbr.sh
```

Secure SSR:
No SSR logs, use a no-logs DNS

```
wget -N --no-check-certificate https://raw.githubusercontent.com/OneHappyForever/shadowsocks_auto/master/shadowsocksR.sh && bash shadowsocksR.sh

```

Encryption: ChaCha20
Obfucation: auth_sha1_v4_compatible/http_simple_compatible

If you want to edit DNS from the default, change it here and restart Shadowsocks:
```
nano /usr/local/shadowsocks/shadowsocks/dns.conf
/etc/init.d/shadowsocks restart
```
