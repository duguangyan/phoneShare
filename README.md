nativeShare
======


nativeShare是一个可以通过javascript直接调用原生分享的工具.

我们知道现在我们无法直接通过js直接跳转到微信和QQ等软件进行分享,但是现在像UC浏览器和QQ浏览器这样的主流浏览器自带一个分享工具,而他们也有自己定义的js接口.我们通过调用浏览器的接口去调用浏览器的分享,从而实现原生分享功能.是不是很酷呢?

该工具具有以下特点:

* 支持原生微博、微信好友、微信朋友圈、QQ好友、QQ空间分享

* 支持调用浏览器更多分享功能

* 注意:目前仅支持手机UC浏览器和QQ浏览器

github项目地址:  [git@github.com:duguangyan/phoneShare.git]



使用方法
--------------------

* 引入CSS文件

``` html
<link rel="stylesheet" href="nativeShare.css"/>
```

* 在需要放分享的地方插入以下代码

``` html
<div id="nativeShare"></div>
```

* 添加配置,并实例化

``` javascript
<script>
    var config = {
        url:'http://du-u.top',// 分享的网页链接
        title:'杜光焱的个人网站',// 标题
        desc:'杜光焱的个人网站',// 描述
        img:'http://b71.photo.store.qq.com/psu?/V134x3kM0Jfkh3/4QM9.FBqiV9L7dtviidPZl9.Ue6Zrhj1aH3NfLutOuw!/b/YcAXZCqcQwAAYiEDYSohRAAA&bo=WALCAQAAAAABBLo!&rf=viewer_4',// 图片
        img_title:'杜光焱的个人网站',// 图片标题
        from:'杜光焱的网站' // 来源
    };
    var share_obj = new nativeShare('nativeShare',config);
</script>
```

截图
--------------------

![分享列表](http://i1.tietuku.com/5e6c8ab36cfb7990.jpg)
![更多](http://i1.tietuku.com/9f391d6e086aecad.jpg)

