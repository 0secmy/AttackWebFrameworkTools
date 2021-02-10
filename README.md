# AttackWebFrameworkTools
使用方法
<h2>工具编写背景:</h2>
<ul>
<li>编写目的：<br>
测试已经公开漏洞
</li>
<li>背景<br>
 在公司内部有些早已经公开的漏洞比如struts2 thinkphp weblogic 这些需要批量测试用网上的工具有C#写的有python java 写的用这些工具都得装一下依赖库。python虽然很方面但是装库确实是很麻烦。另外本人也不擅长python编写最后选择.net来编写
</li>
<li>优点缺点<br>
（1）缺点不跨平台<br>
（2）优点傻瓜是主要导入url即可实现批量测试,能一键getshell监测绝不sql注入或者不是监测
</li>
</ul>
<h2>工具使用</h1>
<ul>
AttackWebFrameworkTools 使用说明<br/>
url.txt 中网站一行一个且必须以http:// https:// 开头<br/>
AttackWebFrameworkTools.exe 所有exp都跑<br/>
AttackWebFrameworkTools.exe -type thinkphp 使用默认线程跑 thinkphp框架漏洞使用说明<br/>
AttackWebFrameworkTools.exe -type thinkphp -thread 200 使用自定义线程 线程跑 thinkphp框架漏洞<br/>
集成漏洞如下(-type参数) <br/>
**thinkphp**<br/>
**weblogic**<br/>
**struts2**<br/>
**hadoop**<br/>
**atlassiancrowd**<br/>
**ueditor**<br/>
**tongdaoa**<br/>
**apacheflink**<br/>
**ruijie**<br/>
**apachedruid**<br/>
**dlink**<br/>
如果会在软件同目录下生产shell.txt。攻击不成功则不会生成
</ul>

<h2>软件使用注意事项</h2>
<ul>
<li>(1)非回显漏洞采用dnslog 验证确保联网。如果在局域网不联网环境下dnslog验证的漏洞全部无法验证。
</li>
<li>(2)遇到postData是jason格式时候必须 Content-type:application/json 而不是默认格式<br/></li>
<li>(3)Dlink漏洞需要有AttackWebFrameworkTools.exe.config 并且一个网站一分钟内最多可以检测三次超过三次即使漏洞存在也检测不到 这个目前反弹shell方式不清楚<br/>
</li>
<li>建议进行针对对性漏洞测试全量跑耗时就容易被waf封<br/></li>
<li>切勿使用工具对网站进行未授权非法攻击,由此一切产生的后果与作者无关!!!!</li>
<li>另外说如果有合适的exp或者poc可以联系我邮箱Anonymous-ghost@qq.com一起携手打造web框架自动化测试工具</li>
</ul>
<h2>上图实测效果</h2>

软件界界面<br/>
![这里随便写文字](https://lofter.lf127.net/1611802266191/huanlesong.jpg)
druid测试批量测试<br/>

ApacheFlink实战png

<h2>注意如果提示软件时间到期可以更改本地时间时间改成2021-02-10-2021-02-30就可以打开软件了</h2>
下载地址
