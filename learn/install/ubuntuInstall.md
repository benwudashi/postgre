## Install（安装）
* Ctrl+alt+T打开终端输入

  `sudo apt-get install postgresql` 
  
  或者`sudo apt-get install postgresql postgresql-contrib`
  
[附：安装示例链接]（https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04#installation） 

## 连接postgre

* 切换到postgres用户 `sudo su - postgres`

  使用psql进入数据库 `psql`
  
  使用\q退出postgre `\q`
  
  使用\l（字母）显示所有数据库 `\l`
  
* Linux下使用service查看数据库启动状态

  #### `sudo service postgres status` 
  
  ####  `sudo service postgres start` 
  
  ####  `sudo service postgres stop` 
  
  ## 一些简单设置
  * 修改postgres用户密码｀ \password postgres ｀
  
  * 端口修改：找到postgresql.conf文件搜索port 修改，默认端口为5432
  
  * 打开日志收集功能:`logging_collector = on`
  
  * 日志路径：`#log_directory = 'pg_log'`
  
  * log file name pattern:`#log_filename = 'postgresql-%Y-%m-%d_%H%M%S.log'`
  
  其他配置参考文件：postgresql.conf.sample
  
