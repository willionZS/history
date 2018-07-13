Mycroft开源demo简单使用<br> <br> <br> 
===========
准备环境<br> <br>
------------
首先，获取Mycroft的源代码程序，可以直接clone或者git（git如下）：<br> 
`cd ~/`<br> 
`git clone --depth=1 https://github.com/MycroftAI/mycroft-core.git` <br> 
`cd mycroft-core`<br>  
`bash dev_setup.sh`<br> 
![bash](https://github.com/willionZS/history/blob/master/mycroft-picture/1bash.png)<br><br>
bash完成如下
![bashed](https://github.com/willionZS/history/blob/master/mycroft-picture/2bashed.png)<br><br>
dev_setup.sh这个脚本为安装依赖项，在ubuntu下，直接bash它等待完成安装即可，其他系统需要根据提示手动安装软件包 <br> <br> <br>


运行Mycroft <br><br>
-------------
Mycroft包里有start-mycroft.sh这个脚本，可以用来启动这个demo，运行如下： <br>
`cd ~/mycroft-core` <br>
`./start-mycroft.sh debug` <br>
![start](https://github.com/willionZS/history/blob/master/mycroft-picture/3start-mycroft.png)<br><br>
"debug"为命令启动后台服务（麦克风，skill模块，消息，音频等系统）以及文本命令行界面(CLI)，你可以使用CLI和Mycroft进行交互，
并查看交互内容和log日志内容 <br>
或者，您可以运行./start-mycroft.sh all以在没有命令行界面的情况下开始服务。稍后您可以使用CLI启动CLI ./start-mycroft.sh cli，后台停止服务如下： <br>
`./stop-mycroft。sh`<br>
启动后，程序会自动连接服务器，如果网速不好，或者没有代理的情况下会显示链接不成功，因此翻墙是必要的，而且速度不能太差
（亲测代理ms达到300之后就会连接失败），启动成功,界面如下：<br>
![sign](https://github.com/willionZS/history/blob/master/mycroft-picture/4sign.png)<br><br>
如图所示，Mycroft会给你提供一个6位数字与字母组合而成的激活码，一长串句子，打引号的字母和数字就是激活码，
你需要使用这个激活码登录到home.mycroft.ai来为你的设备配对然后才能使用：<br>
你可以使用谷歌账号在它的官网登录，然后配对，也可以使用其它账号，在线配对如下：<br>

![sign](https://github.com/willionZS/history/blob/master/mycroft-picture/5online.png)<br><br>
配对成功后，配对网站在线显示如下，并会给你几个示例问题：<br>
![sigin](https://github.com/willionZS/history/blob/master/mycroft-picture/6had.png)<br><br>
点击finish按钮，就可以看到你刚才在线设置好的，属于自己的mycroft：<br>
![thus](https://github.com/willionZS/history/blob/master/mycroft-picture/thus.png)<br><br>
然后这边运行界面，就会有如下提示:now,I am ready for use，表示你的设备以及可以正常运行了：<br><br>
![pair](https://github.com/willionZS/history/blob/master/mycroft-picture/7paired.png)<br><br>
下面是我在使用过程的几个示例，可以问它的名字，你会发现它已经默认自己名字为你刚注册时给它取的名字，以及他还可以唱歌，读新闻，帮你google维基百科<br>
![used](https://github.com/willionZS/history/blob/master/mycroft-picture/8used.png)<br><br>
![sing](https://github.com/willionZS/history/blob/master/mycroft-picture/9sing.png)<br><br>
