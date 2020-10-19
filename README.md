# heimdall-cn
## 序言
一键docker安装heimdall
中文化
国内源修改
## 使用
```

cd /home
git clone https://github.com/odyf/heimdall-cn.git
cd heimdall-cn
docker-compose up
git checkout app/SupportedApps.php
git checkout lan/en/app.php
docker-compose up -d
```

## 注意事项

使用除root以外的用户启动容器 不然会报错





## 使用项目

[linuxserver/heimdall](linuxserver/heimdall)

[Heimdall 大中华镜像源(修改版)](https://gitee.com/sKai-Zhang/Heimdall-List/tree/master)

[土味汉化文件地址](https://pan.baidu.com/s/1OQwK8oY3Q7ZmW4r4eQ-QiQ) 提取码：ijf5



汉化原理：heimdall采用了专门的语言包，找到这个语言包，加上自己的翻译，然后替换即可。

语言包路径：heimdall的语言包路径是在容器内部的 /var/www/localhost/heimdall/resources/lang/ 文件夹下面，我们在heimdall主页设置中能设置的每一种语言，在这个路径中都有一个对应的文件夹，比如说我要替换的德语文件夹的目录就是 /var/www/localhost/heimdall/resources/lang/de/ ，这个目录下就一个文件——app.php