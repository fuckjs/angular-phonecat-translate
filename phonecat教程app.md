# phonecat教程app

这个教程是开始学习angular最好的方式，在这儿你能看到整个angular的相关细节。这个app的功能是用于展示一系列安卓设备的相关参数，你可以过滤产品列表以展示你最感兴趣的内容，同时可以查看每款设备的细节。

原文链接 ：https://docs.angularjs.org/tutorial

![产品展示图片](https://docs.angularjs.org/img/tutorial/catalog_screen.png)

根据以下教程，你可以学习到angular怎样使客户端程序更有效率的运行。
* 使用数据绑定，构建根据用户行为即刻改变视图的动态页面。
* 在不使用Dom操作的情况下让你的视图与你的数据保持同步。
* 使用Karma 和 Protractor进行测试会使你的流程更加的简单。
* 学习使用依赖注入和服务来让你常用的任务更加简单，例如在你的app内获取数据。

当你完成此教程，你能达到以下水平。
* 创建一个能够在所有主流浏览器中运行的动态app
* 通过数据绑定来让你的数据和视图联动
* 使用karma进行单元测试
* 使用Protractor来结束单元测试
* 把应用逻辑从模板移入到控制器
* 通过angular服务从服务器端获取数据
* 使用ng-animate为你的app添加动画
* 获取更多关于angular的资源

## 开始
以下部分讲解了如何构建开发环境。如果你只是想你可以直接去第一步[Step 0 - Bootstrapping](https://docs.angularjs.org/tutorial/step_00).

## 和代码一起工作
你可以跟随此教程在自己电脑上敲代码，这样就可以得练习的机会。

这个项目使用git进行代码管理。但是关于git你只需要了解几个常用的命令即可。

### 安装git

### 下载angular.phonecat
通过以下命令从github上下载项目

> git clone --depth=14 https://github.com/angular/angular-phonecat.git

这个命令会在你本地库里添加相关目录。

		--depth=14 选项告诉git只需拉取最近提交14次提交。这样会使下载量变小一些。

将你的目录调整到当前

> cd angular-phonecat

之后，我们都将在这个目录里进行操作。
