#关注H5开发社区公众号，获取更多微信小程序开发教程
![](https://mmbiz.qpic.cn/mmbiz_png/OzyYXjBCAYia064da1bBbSMpLFGCTLqO9o5UMW7CWQzAYNjelDL5f8Dyofh73sHgjBbhm9lNnh3eEx1Anuol96w/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)
### 主要特性

- 想学一下微信小程序，发现文档这东西，干看真没啥意思。所以打算自己先动手撸一个。摩拜单车有自己的小程序，基本功能都有，方便又小巧，甚是喜爱。于是我就萌生了一个给ofo共享单车撸一个小程序(不知道为啥ofo没有小程序)的想法。Let's do it!

由于本文篇幅过长，影响浏览体验，我对这篇文章做了一下拆分，修正了一些错误

# 先上一波效果图：

![](https://upload-images.jianshu.io/upload_images/2795762-397166cf2df4cd93.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)
![](https://upload-images.jianshu.io/upload_images/2795762-5b0f0b7ef9339251.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)
![](https://upload-images.jianshu.io/upload_images/2795762-fab144940facabf5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)


**目录 (Table of Contents)**
pages文件夹下存放着小程序所有的业务页面；

index文件夹就是一个页面，index.wxml是页面的结构文件，类似html。

index.wxss是页面的样式，其实就是css；index.js是页面的逻辑，数据请求与渲染都是都在这个页面完成。

logs文件夹存放着小程序开发日志，目前暂时用不到。

utils.js可以编写自己的JavaScript插件。

app.js处理全局的一些逻辑，比如定义全局变量存放获取的用户信息，这样每个页面都可以获取用户信息。

app.json 是全局配置文件，比如设置标题栏的背景色等。

app.wxss 存放页面的公共样式，如果多个页面需要用到同一样式，就可以写在这里。

项目按钮显示预览二维码，用于真机调试。必须真机调试测试代码

### End