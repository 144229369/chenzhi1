# chenzhi1

>这是一个简单的全栈web APP,基于Deno + Vue + Mysql.

功能：

##Client

>运用在Brower里的应用程序“code” （html + js + css）

##Server（1）

>运行在Linux上的web服务应用程序

-响应浏览器HTTP请求

'''sh
#安装unzip解压工具
sudo apt install zip
#安装deno
curl -fsSL https://deno.land/x/install/install.sh | sh
#拷贝二进制文件
sudo cp .deno/bin/deno /usr/bin
#检查安装是否成功
deno --version

'''
##启动服务
'''
deno run --allow-read --allow-net mod.js
'''
##DataBase

>持久化数据，保存Brower浏览器端用户需要的数据

- client html页面，用户点击，发起HTTP请求
- server层 api：相应client端用户HTTP请求（通过dano 三方库 实现mysql使用）
- Linux系统：'install mysql' 服务
- 数据库：创建用户，创建表。插入数据
