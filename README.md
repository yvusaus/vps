更新及安装组件
```
apt update && apt install -y curl wget
```
一键启用BBR
```
echo "net.core.default_qdisc=fq_pie" > /etc/sysctl.d/99-bbr.conf && \
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.d/99-bbr.conf && \
sysctl --system
```
安装AnyTLS
```
anpt="" bash <(curl -Ls https://raw.githubusercontent.com/yonggekkk/argosbx/main/argosbx.sh)
```
重启
```
reboot
```
显示
```
agsbx list
```
卸载
```
agsbx del
```

建议配合SSH一键脚本命令生成器网页使用：
https://yonggekkk.github.io/argosbx/

realm转发面板
```
curl -L https://host.wxgwxha.eu.org/https://github.com/wcwq98/realm/releases/download/v2.1/realm.sh -o realm.sh && chmod +x realm.sh &&  ./realm.sh
```
```
nano /root/realm/web/config.toml
```
安装 MTProxy
```
rm -rf /home/mtproxy && mkdir /home/mtproxy && cd /home/mtproxy
curl -fsSL -o mtproxy.sh https://github.com/ellermister/mtproxy/raw/master/mtproxy.sh
bash mtproxy.sh
```
一键更改roo密码
```
wget -N https://gitlab.com/rwkgyg/vpsroot/raw/main/root.sh && bash root.sh
```
