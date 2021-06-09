# linux-config
my linux config files

## Path

- `.bash_aliases` >> ~/.bash_aliases
- `.inputrc` >> ~/.inputrc
- `proxychains.conf` >> /etc/proxychains.conf

## Configurations

### proxychains-ng

```bash
$ git clone https://github.com/rofl0r/proxychains-ng
$ cd proxychains-ng
$ ./configure --prefix=/usr --sysconfdir=/etc
$ make
$ sudo make install
$ sudo make install-config # 安装proxychains.conf配置文件
$ sudo vim /etc/proxychains.conf
[ProxyList]
# add proxy here ...
# meanwile
# defaults set to "tor"
socks5  127.0.0.1 1080
```

## Git Proxy

```bash
$ git config --global http.proxy 'socks5://127.0.0.1:1080'
```

