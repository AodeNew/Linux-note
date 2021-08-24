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
## 为什么发起这个项目？
几个月前，我参加了一场AWD攻防比赛，发现提前收集POC对比赛有好处而且在收集这些payload的同时，也能学到许多东西.
## 问题反馈 
在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流
* 邮件(MrSm1th@163.com)
### 如果你想共同维护这个项目?
* 联系邮箱(MrSm1th@163.com)
