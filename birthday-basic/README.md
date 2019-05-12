## birthday-basic

### 说明
这是我最开始写的三个静态网页，你可以将其定制之后送给自己的朋友/对象/送完还是朋友的朋友/送完就变成对象的朋友，2333

因为只是我最开始送人所写的网页。所以会有不少问题，如果在使用过程中发现这些问题请见谅。

### 在线预览
http://119.23.212.211:8080/birthday-basic/  
用户名：123 密码：123

### 使用前提
如果你具备前端开发的相关经验，那么可以自由地在这个模板上进行相关的修改，相信我当年写的代码能把你气个半死（手动滑稽，我现在自己看了也生气）

如果你不具备任何前端开发的经验，那么或许可以考虑换个东西送？

如果你只是简单了解相关知识，那么你可以阅读下面的引导来了解这个模板。

### 模板介绍
#### 修改密码
 在当前目录下，有js/login.js文件：
 ```javascript
 //修改此处的123,123即可修改登录的用户名和密码
 if(userName=="123" &&  pwd=="123"){
   event.preventDefault();
   $('form').fadeOut(500);
   $('.wrapper').addClass('form-success');
   setTimeout(function(){location.href="BirthdayCake.html";},2000);
 }
 ```

#### 替换memories页面文字和图片
以第三屏为例：
```html
<!--第三屏-->

<div class="section">
    <!-- 下面两个div分别实现的左边那条轴和那个小球 -->
    <div class="timeline"></div>
    <div class="timepoint21"></div>
    <div class="ly-box21">
        <div class="ly-txt21">
            <!-- 这里更改日期 -->
            201X-1X-2X
        </div>
        <div class="ly-txt22">
          <!-- 这里更改内容，段落、换行用<p></p>包裹起来 -->
           <p> XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</p>
           <p>XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</p>
        </div>
        <div class="ly-imgbox21">
          <!-- 这里更改图片，图片请先改好对应的名字并且放到img文件夹下面
              如果你不懂css，那么最好就裁剪图片至合适大小为止
              如果你会css，那么可以根据class名字去修改对应css的宽度设置-->
          <img class="ly-img21" src="img/2014.11.26-1.png">
        </div>
    </div>
    <div class="ly-triangle21"></div>

    <div class="ly-box22">
        <div class="ly-txt23">
          <!-- 与上面类似，不再多说 -->
            201X-1X-1X
        </div>
        <div class="ly-txt24">
            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
        </div>
        <div class="ly-imgbox22">
          <img class="ly-img22" src="img/2014.12.19-1.png">
        </div>
    </div>
    <div class="ly-triangle22"></div>

     <div class="ly-box23">
        <div class="ly-txt25">
            201X-1X-2X
        </div>
        <div class="ly-txt26">
            XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
        </div>
        <div class="ly-imgbox23">
          <img class="ly-img23" src="img/2014.12.20-1.jpg">
        </div>
    </div>
    <div class="ly-triangle23"></div>
</div>
```

## 如何给别人看
1. 打成压缩包发给别人  
2. 部署至云服务器或者虚拟主机  
    1. 部署云服务器需要拥有一台自己的云服务器。部署方式有很多种，这里推荐两种：  
        - 使用Tomcat部署:
    在服务器下载解压tomcat，解压后打开webapps文件夹，然后新建一个英文名称的文件夹(称为路径名)，下载此项目后将当前目录（注意，只拷贝文件，含有index.html在内的这些html和css，js之类的拷贝到刚才新建的文件夹内，重启tomcat即可。）
        - 使用nginx部署：
    方式类似，不扯了，可以自行去百度查。
    2. 部署至虚拟主机，在虚拟主机购买商处会有教程

如果需要用域名访问，请先去购买域名，然后按照教程进行解析。

## 注意点
请使用Google Chrome浏览器！

没有手机版！


## 其它问题
有问题请发邮件至 guoxiaofeng_2015@163.com,公有问题我会继续更新在readme

## 开发计划
1. 修改Memories页面布局，保证宽屏适应。
2. 注意浏览器兼容性。
3. 注意在手机上的表现。
4. memories模块动态生成。  
这些都是有空之后会慢慢做的，欢迎持续关注~
