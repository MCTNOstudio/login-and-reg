此程序使用CC（A Creative Commons license）协议开源，作者为学个锤子（QQ2773660966），请自行更换登录界面UI，
具体方法：将login.html改名为login_bk.html，然后将login1-5.html改成login.html
学个锤子blog：http://blog.mctno.com/
index.html可以直接阉了，这个是初始化引导页面，删除以后请自行访问http://你的域名/install
后台初始化、前端index.html界面UI为小皮原创
此登录系统为MCTNO工作室开发，无任何抄袭，如有侵权，请联系niuziyi@mail.mctno.com，看到以后会第一时间删除此系统
-----**FAQ**-----
1.Q:挂在网站上就报错,本地就行
A:请检查php环境是否支持mysqli，是否已安装mysql数据库，php是否已打开，如果报错为<?php开头，即说明php没打开，如为warning或error开头，请联系学个锤子解决
2.Q:我想对接别的网页，应该怎么对接？
A:首先把文件后缀改成php,然后在开头加一个
<?php
$pd = @cookie(login);
$user = @cookie(user);
if($pd != TRUE){
header('location:login.html'); 
}
?>
用户名为$user
3.Q:我不知道我的php版本怎么办
A:请先访问http://你的域名/install/config.php 如果加载出来了就说明支持php，请查看是否支持mysql，mysqli,检查完后请删除config.php，防止骇客骇入
