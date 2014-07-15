garage
======
the step to install the garage

1. git clone git://github.com/shiqianmiao/garage.git
2. clone完毕后，进入garage目录，配置里面的config.json文件，主要修改里面的一些目录和版本号缓存的memcached的配置，目录也可以不改直接用默认目录结构。
3. 默认目录结构为  xxx/garage/src/test/..... 
4. 如果不想叫test的话，可以修改config.json的同时，进入garage/node_modules/grunt-crane/tasks, 修改里面的build.js
5. 目录都整理好之后，需要安装nodejs，去http://nodejs.org 下载最新的源码安装包，解压，./configure; sudo make; sudo make install;     安装完毕。执行node命令测试是否成功安装。
6. 完了，安装 node的npm， ubuntu下面可以：sudo apt-get install npm 搞定。
7. 然后安装 grunt-cli。命令：npm install -g grunt-cli。
8. 此时进入garage目录，执行 grunt build即可开始编译test中的代码到  garage/build/test/中，配置nginx指向build即可。
