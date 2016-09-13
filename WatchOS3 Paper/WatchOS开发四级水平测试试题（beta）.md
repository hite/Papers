## WatchOS开发四级水平测试试题（beta）
***（本试题大纲限于watchOS 3）***
###### 名词约定
watchOS开发中涉及到的主体包括，运行在iPhone的iOS程序（以下称`iOS app`），运作在Apple Watch端的App（以下简称`Watch app`)，运行在Apple Watch端的扩展（以下简称`WatchKit extension`）。

*（点击+号查看答案）*

### 基础题

1. 关于以下宣传广告，从技术层面看，哪个活动文案是最正确的.（ <input style="width:50px;" type="text" name="answer"/> ）
	<ol type="A">
	<li>
	<a style="cursor:hand;text-decoration:none;" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png"/>
	</a>
	</li>
	<li>
	<a style="cursor:hand;text-decoration:none;" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badb4009b0b.png"/>
	</a>
	</li>
	<li>
	<a style="cursor:hand;text-decoration:none;" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badbae27c8e.png"/>
	</a>
	</li>
	<li>
	<a style="cursor:hand;text-decoration:none;" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badbcab1652.png"/>
	</a>
	</li>
	<li>
	<a style="cursor:hand;text-decoration:none;" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badc071b4f0.png"/>
	</a>
	</li>
	</ol>
<div class="w-answer-wrap">
<button type="submit" style="width:100px;height:26px;margin:0 5px;" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content">
**答案是（D，E）试题解析**  
事实上，苹果本身从来没有称呼iWatch的说法。iWatch只是媒体和大众对苹果新产品命名的一种猜测。按照iPhone，iPod，iMac的管理，watch应该iWatch。但是从john ivy之后，i字头产品已经没有了，而取而代之是去话。如iPhoto被Photos取代，许久不更新的iMac系列。新产品以Air、Pro、Plus等更时髦的叫法。   
`On September 9, 2014, Apple unveiled its long-rumored wearable device, the Apple Watch. While many expected the wearable to be called the "iWatch," Apple actually opted to use the Apple symbol () followed by "Watch" for the device's name.`
</div>
1. The Apple Watch is designed to be both functional and fashionable, available in two sizes of 38mm and 42mm , with eight different casing materials and dozens of interchangeable band options in a variety of colors . 在[watchOS Human Interface Guidelines](https://developer.apple.com/watch/human-interface-guidelines/visual-design/)文档里有 ![](http://ooo.0o0.ooo/2016/08/26/57c01c761f92f.jpg)图示。试阅读上述资料，回答以下问题。第一：38mm和42mm的屏幕尺寸是分别是多少？（ <input style="width:50px;" type="text" name="answer"/> ）
<ol type="A">
	<li>
	1.3 inches
	</li>
	<li>
	1.4 inches
	</li>
	<li>
	1.5 inches
	</li>
	<li>
	1.6 inches
	</li>
	<li>
	1.7 inches
	</li>
	</ol>
	<div class="w-answer-wrap">
	第二：38mm和42mm的Apple Watch 的DPI分别是多少？（ <input style="width:50px;" type="text" name="answer"/> ）；   
<ol type="A">
	<li>
	302
	</li>
	<li>
	290
	</li>
	<li>
	326
	</li>
	<li>
	329
	</li>
	</ol>
<button type="submit" style="width:100px;height:26px;margin:0 5px;" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content">
**答案是（A，C），（C，C）试题解析**  
首先明确，Apple Watch的文档里标明的38mm，是指整个表盘的高度，**不是**屏幕高度。下图是官方提供的38mm Apple Watch的measurements图片。 <a title="点击查看大图" alt="official Apple Watch measurements" style="cursor:hand;text-decoration:none;" href="http://ooo.0o0.ooo/2016/08/26/57c0259163d22.jpeg" target="_blank">
		<img style="width:100%0px;" src="http://ooo.0o0.ooo/2016/08/26/57c0259163d22.jpeg"/>
	</a>来源 [Rene Ritchie](https://twitter.com/reneritchie/status/599397428618493953/photo/1)、Apple官方文档[Band-Design-Guidelines-for-Apple-Watch](https://developer.apple.com/watch/bands/Band-Design-Guidelines-for-Apple-Watch.pdf)。<br/>其次，明确PPI的计算公式，根据博主Sebasiten Gabriel 叙述```DPI or Dots Per Inch is a measure of spatial dot density initially used in print. It's the number of ink drops your printer can put in an inch. The more dots per inch, the sharper your image.
This concept is applies to computer screens under the name PPI for Pixels Per Inch. Same principle: It counts the number of pixels your screen displays per inch. The name DPI is also used in screens.```， 假设`P` 是代表Pixels，`I`代表Inches，且`1Inch = 2.54cm`, 所以的表盘对角线的英寸是`Math.sqrt(Math.pow(21.22,2)+Math.pow(26.54,2))/25.4 = 1.3378`。根据Band Design Guide中的尺寸。得知42mm的Active Area为`30.42 * 24.66`，所有同理可得42mm的对角线尺寸是` = 1.54 ~ 1.5`，所以答案是*A和C*；对角线像素长度 = `Math.sqrt(Math.pow(340,2) + Math.pow(272,2)) = 435.4`，得到38mm的表屏幕尺寸为`435.4/`，计算高度方向的PPI,`P = 340px, I = 1.3378 `，所以得到`PPI = 435.4/1.3378 = 325.459 ~ 326 `。因为苹果官网上没有明确指出38mm和42mm的范围，导致很多人误解，以为是指Active Area区域的高度，所以有`290\302`这两种PPI。有些动手能力强的网友尝试自己用[游标卡尺测量](https://ooo.0o0.ooo/2016/08/30/57c57eb9c074b.jpg)，得出正确的结论。不过这个方法有点耿直。
</div>
1. Apple Watch如果没有配对的iPhone功能是有限的，如果需要iPhone配对，可采用蓝牙*Bluetooth 4.0*和Wi-Fi *(802.11b/g/n 2.4GHz）*两种方式来通讯，根据官网资料[About Bluetooth and Wi-Fi on Apple Watch](https://support.apple.com/en-hk/HT204562)所述，没有可连接WiFi时，Apple Watch和iPhone的链接是通过蓝牙来通讯的。阅读以上资料，假设使用环境为普通的室内办公环境，请选择Apple Watch和iPhone可正常的最远能相隔多远。（ <input style="width:50px;" type="text" name="answer"/> ）
<ol type="A">
	<li>
	10米左右
	</li>
	<li>
	30米左右
	</li>
	<li>
	70米左右
	</li>
	<li>
	100米左右
	</li>
	</ol>
<button type="submit" style="width:100px;height:26px;margin:0 5px;" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content">
**答案是（C）试题解析**  
这个问题，可能没有标准答案。`Bluetooth uses radio waves (short-wavelength UHF to be exact) between 2.4 and 2.485 GHz in the ISM band. Long story short, that means that a Bluetooth signal can be interrupted by Wi-Fi signals, satellite dishes, certain external monitors, microwaves, bodies, certain electronics, etc.` ，所以在不同的环境下测试的结果可能不同，根据我自己的测试有效距离是30m，而其他人测试的结果可能是` up to 330 feet (100 meters) `，这个结论来自[What is the Apple Watch connection distance to iPhone?](http://bradymower.com/apple-watch-connection-distance-iphone/)，类似的讨论也有，比如这个讨论帖，[What's the farthest distance one can go before the Watch loses connection with the iPhone?](http://forums.imore.com/apple-watch/334781-what-s-farthest-distance-one-can-go-before-watch-loses-connection-iphone.html)。在翻阅了其他关于蓝牙有效距离的之后，发现如下结论:`有效距离和功率相关`，![](http://ooo.0o0.ooo/2016/09/13/57d76c66ba60d.jpg)`Officially Class 3 radios have a range of up to 1 metre (3 ft), Class 2, most commonly found in mobile devices, 10 metres (33 ft), and Class 1, primarily for industrial use cases,100 metres (300 ft).[3] Bluetooth Marketing qualifies that Class 1 range is in most cases 20–30 metres (66–98 ft), and Class 2 range 5–10 metres (16–33 ft).[2]`,而Apple Watch采用的是*Bluetooth 4.0*，根据表格![](http://ooo.0o0.ooo/2016/09/13/57d76cefbc865.jpg)可见应该最大是69m，而`Bluetooth Marketing qualifies that Class 1 range is in most cases 20–30 metres (66–98 ft)`，可侧面说明应该是30m左右。以上资料来自 wikipedia，[Bluetooth词条](https://en.wikipedia.org/wiki/Bluetooth#Setting_up_connections)
</div>
1. 请阅读以下资料，回答问题。，。。。请选择选择下面哪项描述正确。（ <input style="width:50px;" type="text" name="answer"/> ）
<ol type="A">
	<li>
	1.3 inches
	</li>
	<li>
	1.4 inches
	</li>
	<li>
	1.5 inches
	</li>
	<li>
	1.6 inches
	</li>
	<li>
	1.7 inches
	</li>
	</ol>
<button type="submit" style="width:100px;height:26px;margin:0 5px;" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content">
**答案是（A，C），（C，C）试题解析**  
回答这个问题之前需要搞清楚什么是xcode的构建，见[贴文](http://gcblog.github.io/2016/03/12/Xcode多工程联编及工程依赖/)
首先明确，Apple Watch的文档里标明的38mm，是指整个表盘的高度，**不是**屏幕高度。下图
</div>


