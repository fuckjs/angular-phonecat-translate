## 1 static template 静态模板
为了论证angular如何接管普通的html文件，你需要创建一个静态html页面，然后检查怎样能把这个页面变成模板。

这次你会在页面上为两款手机添加一些基本信息。

在你的项目里更改版本	
>	git checkout -f step-1

以下是相关的变化

app/index.html:
	
	<ul>
	  <li>
	    <span>Nexus S</span>
	    <p>
	      Fast just got faster with Nexus S.
	    </p>
	  </li>
	  <li>
	    <span>Motorola XOOM™ with Wi-Fi</span>
	    <p>
	      The Next, Next Generation tablet.
	    </p>
	  </li>
	</ul>
    