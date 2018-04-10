# YankeeBBR
来自Loc大佬Yankee魔改的BBR的Debian一键安装包


部分商家的VPS可能会遇到换内核之后无法启动系统的情况，所以请运行脚本前一定要备份好重要数据！！

安装使用
wget -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/YankeeBBR/master/bbr.sh && bash bbr.sh install
安装过程中如果出现这张图片，请选择NO 来删除其他内核：

安装过程中如果出现这张图片，请选择NO 来删除其他内核：

bbr2.png
然后根据提示重启系统。
重启完成后，运行

bash bbr.sh start
即可启动魔改版BBR。

查看魔改BBR状态
sysctl net.ipv4.tcp_available_congestion_control
如果看到有 tsunami 就表示开启成功！

bbr3.png
