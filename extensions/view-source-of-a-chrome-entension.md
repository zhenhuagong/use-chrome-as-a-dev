来自Paul Irish的[Github Gist](https://gist.github.com/paulirish/78d6c1406c901be02c2d)。

有三种方法来查看一个Chrome插件的源码。

###命令行
在命令行下载插件，并保存成`.zip`格式。解压之后就看到源码了。
```
extension_id=jifpbeccnghkjeaalbbjmodiffmgedin   # change this ID
curl -L -o "$extension_id.zip" "https://clients2.google.com/service/update2/crx?response=redirect&os=mac&arch=x86-64&nacl_arch=x86-64&prod=chromecrx&prodchannel=unknown&prodversion=44.0.2403.130&x=id%3D$extension_id%26uc"
unzip -d "$extension_id-source" "$extension_id.zip"
```

###使用`CRX Viewer`插件
在[Chrome Webstore](https://chrome.google.com/webstore)里查找并安装[Chrome extension source viewer](https://chrome.google.com/webstore/detail/chrome-extension-source-v/jifpbeccnghkjeaalbbjmodiffmgedin?hl=en)，它还是开源的：[Github Repo](https://github.com/Rob--W/crxviewer)。

安装之后，在Chrome Webstore中点开某个插件的页面，然后你会在浏览器地址栏右侧发现一个黄色的`CRX`按钮。点击它，就可以查看这个插件的源码了。

![](https://cloud.githubusercontent.com/assets/729479/9938215/e3262910-5d96-11e5-89f3-3b16e69f8dab.png)

###直接查看本地安装的插件

* 已安装的插件的本地文件夹
    - 在浏览器地址栏输入`chrome://version`，会显示当前Chrome浏览器的各种属性信息
    - 找到`Profile Path/个人资料路径`属性，后面的路径就是你需要的，复制它
    - 打开刚刚复制的那个本地文件夹，然后打开下面的`Extensions`子目录
* 你会发现`Extensions`子目录下的文件夹名字像天书似的
* 查看每个文件夹下的`manifest.json`文件，里面有`name`属性，就是你安装的插件的名字。这样就能把本地插件目录和插件名字对应起来了。

![](https://cloud.githubusercontent.com/assets/39191/9500889/d7ffe65a-4bdc-11e5-9cfd-06ac0cbe5497.png)

