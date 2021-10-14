# Linux 常用命令  不断更新中
* 修改网络配置文件，文件地址：/etc/sysconfig/network-scripts/ifcfg-eth0
* 主要修改以下配置：
* TYPE=Ethernet               //网络类型
* BOOTPROTO=static            //静态IP
* DEVICE=ens00                //网卡名
*  IPADDR=192.168.1.100        //设置的IP
*  NETMASK=255.255.255.0       //子网掩码
*  GATEWAY=192.168.1.1         //网关
*  DNS1=192.168.1.1            //DNS
*  DNS2=8.8.8.8                //备用DNS
*  ONBOOT=yes                  //系统启动时启动此设置
* 修改保存以后使用命令重启网卡：service network restart
* 正向连接
假设我们攻击了一台机器，打开了该机器的一个端口，攻击者在自己的机器去连接目标机器（目标ip：目标机器端口），这是比较常规的形式，我们叫做正向连接。远程桌面、web服务、ssh、telnet等等都是正向连接。
