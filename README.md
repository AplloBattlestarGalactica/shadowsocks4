# shadowsocks4
* git clone到自己的vps
* 给文件加权限
* 首先执行./ss.sh
* 建议选择ssr
* 然后执行./bbr.sh
* 开启bbr需要kvm内核


Shadowsocks-Python 版：
/etc/init.d/shadowsocks-python start | stop | restart | status

ShadowsocksR 版：
/etc/init.d/shadowsocks-r start | stop | restart | status

Shadowsocks-Go 版：
/etc/init.d/shadowsocks-go start | stop | restart | status

Shadowsocks-libev 版：
/etc/init.d/shadowsocks-libev start | stop | restart | status

### 端口
* -A INPUT -p tcp -m state --state NEW -m tcp --dport 53 -j ACCEPT
* -A INPUT -p udp -m state --state NEW -m udp --dport 53 -j ACCEPT
* -A INPUT -p tcp -m state --state NEW -m tcp --dport 80 -j ACCEPT
* -A INPUT -p udp -m state --state NEW -m udp --dport 80 -j ACCEPT

