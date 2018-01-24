# rclone
#::初始化配置
# rclone config
 
#::挂载为磁盘
# rclone mount DriveName:Folder LocalFolder --copy-links --no-gzip-encoding --no-check-certificate --allow-other --allow-non-empty --umask 000
 
#::卸载磁盘
# fusermount -qzu LocalFolder
--------------------------------------------------
自启动
使用方法:
1.复制内容,注意文本格式(UNIX).
2.将其重命名为rcloned(只要不是rclone就可以).
3.填好REMOTE和LOCAL,复制到/etc/init.d文件夹内.
4.运行初始化命令:bash /etc/init.d/rcloned init
5.使用 bash /etc/init.d/rcloned start 挂载.
6.使用 bash /etc/init.d/rcloned stop 卸载.
