# SEU_Lecture_Robber

研究生要听满8场人文讲座，线上讲座十分难抢，一般十秒钟就抢光了，隐隐之中感觉有人用了脚本抢讲座。

代码主要贡献自https://github.com/Meoooww/fetch_lecture ，在他的基础上进行了整理，并借此学习了些Web知识。

流程如下：

1. 先进行一次登录请求以获取登录表单，其中比较重要的是密码的加密方式（AES对称加密）
2. 建立一个会话对象，利用获取到的登录表单，填入自己的用户名和加密和的密码，利用POST方式请求登录
3. 爬取讲座ID和讲座预约时间
4. 利用讲座ID向服务器发送POST请求，进行讲座预约
5. 多线程实现

这个项目我测试了，登录都没有问题，但是现在的预约讲座是要输入**图片验证码**了，我不知道这个该如何解决，希望有大佬可以指导一下

