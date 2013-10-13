lnmp_auto - auto build lnmp environment

# lnmp_auto介绍
+ 自动搭建Linux+Nginx+PHP+Mysql的环境
+ Nginx默认版本1.4.3
+ PHP默认版本5.5.4
+ Mysql默认版本5.1.72
+ 各安装版本可在配置中进行替换

# lnmp_auto环境
+ 已在Centos 64bit和32bit上测试过

# lnmp_auto目录结构

```bash
lnmp_auto
 | - auto #可执行文件
      |- config #配置文件
      |- mysql #mysql的安装和配置
      |- nginx #nginx的安装和配置
      |- options #参数的处理
      |- php #php的安装和配置
      |- selinux #selinux的安装和处理
 | - binary #生成的二进制文件
 | - dev  #开发过程使用的小脚本，没有用
 | - check  #检测脚本
 | - download #下载文件存放位置
 | - lnmp_auto #入口执行脚本
```

# lnmp_auto使用
## 下载lnmp_auto

记住设置目录和路径的权限

## 运行lnmp_auto

直接运行lnmp_auto
### 会执行下面的操作
+ 会在lnmp_auto中下载对应的源文件
+ 自动生成可执行的二进制代码
+ 将文件挂载为服务

## 额外说明点
mysql的用户名密码为root/lnmp_auto
启动服务等可以使用
/etc/init.d/mysql start/stop/restart
/etc/init.d/php-fpm start/stop/restart
/etc/init.d/nginx start/stop/restart

# License
[The MIT License (MIT)](http://opensource.org/licenses/MIT)

Copyright (c) 2013 Jianfeng Ye

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
