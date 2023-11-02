## 固件编译和下载
1. 本仓库基于armbian官方源码库<a href="https://github.com/armbian/build/">https://github.com/armbian/build/</a>进行编译，特此感谢。
2. 云编译代码修改自<a href="https://github.com/ophub/amlogic-s9xxx-armbian/">https://github.com/ophub/amlogic-s9xxx-armbian/</a>，特此感谢。
## 刷机注意事项
1. 下载安卓固件（参考<a href="https://github.com/ophub/amlogic-s9xxx-armbian/issues/1332">这里</a>）
2. USB Burning Tool刷入安卓固件（还是参考<a href="https://github.com/ophub/amlogic-s9xxx-armbian/issues/1332">这里</a>）
3. 下载armbian<a href="https://github.com/w2xg2022/actions4ty1608/releases/download/Armbian_bullseye_save_2023.06/Armbian_23.08.0_amlogic_s905l3b-ip103h_bullseye_5.15.116_server_2023.06.10.img.gz">固件</a>
4. 用<a href="https://github.com/pbatard/rufus/releases/tag/v4.1">Rufus</a>将armbian固件写入U盘或TF卡，安卓操作U盘开机，开机时要尽快将U盘或TF卡接上接口
5. 在路由器中找到分配到的动态IP，SSH登录后运行armbian-install以写入emmc，Device ID选122、Filesystem选ext4
6. 依照屏幕提示关机、拿掉U盘或TF卡，即可从emmc开机和运行
Device ID选122：
## 固件默认信息
1. 默认IP：DHCP，因为HDMI无法工作，请在路由器查找分配的动态IP
2. 默认管理员账号：root
3. 默认管理员密码：1234
