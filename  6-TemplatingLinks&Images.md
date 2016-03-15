#

在这一步，你会为手机添加缩略图。至于链接，现在为止，还没有添加。在随后的几步里，你会看到目录手机里的额外信息。

我们注意到phones.json文件包含了每款手机的独立的ID和图片链接.图片的url指向app/img/phones/目录。

> app/phones/phones.json

	[
	  {
	    ...
	    "id": "motorola-defy-with-motoblur",
	    "imageUrl": "img/phones/motorola-defy-with-motoblur.0.jpg",
	    "name": "Motorola DEFY\u2122 with MOTOBLUR\u2122",
	    ...
	  },
	  ...
	]

##　模板
> app/index.html:
...
        <ul class="phones">
          <li ng-repeat="phone in phones | filter:query | orderBy:orderProp" class="thumbnail">
            <a href="#/phones/{{phone.id}}" class="thumb"><img ng-src="{{phone.imageUrl}}" alt="{{phone.name}}"></a>
            <a href="#/phones/{{phone.id}}">{{phone.name}}</a>
            <p>{{phone.snippet}}</p>
          </li>
        </ul>
...

为了动态生成能够到详情页的链接，我们使用双大括号的形式作为a标签的href属性。在第2步的时候，我们曾经把{{phone.name}}作为元素的内容；现在，我们使用{{phone.id}}作为元素的属性。

同时，我们使用拥有ngSrc指令为img标签引入图片。这个指令不会使angular表达式停留在他原始的意思上，会把它转化成一个实际的url。


