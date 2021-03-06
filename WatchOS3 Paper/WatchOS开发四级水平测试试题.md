## WatchOS开发四级水平测试试题
名词约定
>运行在iPhone的iOS程序（以下称`iOS app`）；运作在Apple Watch端的App（以下简称`Watch app`)；运行在Apple Watch端的扩展（以下简称`WatchKit extension`）。

（本试题大纲限于watchOS 3，答案示例如：A,E）

<input type="button" value="开始答题" name="start" id="start"/><span style="color:green;" id="timer"></span>


1. 关于以下宣传广告，从技术角度看，哪个活动文案是最正确的.（ <input class="w-answer_inputer" type="text" name="answer"/> ）
	<ol class="innerList" type="A">
	<li>
	<a class="w-view_img" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png"/>
	</a>
	</li>
	<li>
	<a class="w-view_img" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badb4009b0b.png"/>
	</a>
	</li>
	<li>
	<a class="w-view_img" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badbae27c8e.png"/>
	</a>
	</li>
	<li>
	<a class="w-view_img" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badbcab1652.png"/>
	</a>
	</li>
	<li>
	<a class="w-view_img" href="http://ooo.0o0.ooo/2016/08/22/57bad8e11652c.png" target="_blank">
		<img style="width:300px;" src="http://ooo.0o0.ooo/2016/08/22/57badc071b4f0.png"/>
	</a>
	</li>
	</ol>
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是（D，E）试题解析**  
事实上，苹果本身从来没有称呼iWatch的说法。iWatch只是媒体和大众对苹果新产品命名的一种猜测。按照iPhone，iPod，iMac的管理，watch应该iWatch。但是自从苹果的设计由John Ivy掌舵之后，i字头产品已经没有了，而取而代之是去i话。如iPhoto被Photos取代，许久不更新的iMac系列。新产品以Air、Pro、Plus等更时髦的叫法。   
`On September 9, 2014, Apple unveiled its long-rumored wearable device, the Apple Watch. While many expected the wearable to be called the "iWatch," Apple actually opted to use the Apple symbol () followed by "Watch" for the device's name.`
</div>
1. The Apple Watch is designed to be both functional and fashionable, available in two sizes of 38mm and 42mm , with eight different casing materials and dozens of interchangeable band options in a variety of colors . 在[watchOS Human Interface Guidelines](https://developer.apple.com/watch/human-interface-guidelines/visual-design/) 文档里有两种size的平面图。 ![](http://ooo.0o0.ooo/2016/08/26/57c01c761f92f.jpg)图示。阅读上述资料，试回答以下问题。第一：38mm和42mm的屏幕尺寸是分别是多少？（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
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
	第二：38mm和42mm的Apple Watch 的DPI分别是多少？（ <input class="w-answer_inputer" type="text" name="answer"/> ）；   
<ol class="innerList" type="A">
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
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是（A，C），（C，C）试题解析**  
首先明确，Apple Watch的文档里标明的38mm，是指整个表盘的高度，**不是**屏幕高度。下图是官方提供的38mm Apple Watch的measurements图片。 <a title="点击查看大图" alt="official Apple Watch measurements" class="w-view_img" href="http://ooo.0o0.ooo/2016/08/26/57c0259163d22.jpeg" target="_blank">
		<img style="width:100%0px;" src="http://ooo.0o0.ooo/2016/08/26/57c0259163d22.jpeg"/>
	</a>来源 [Rene Ritchie](https://twitter.com/reneritchie/status/599397428618493953/photo/1)、Apple官方文档[Band-Design-Guidelines-for-Apple-Watch](https://developer.apple.com/watch/bands/Band-Design-Guidelines-for-Apple-Watch.pdf)。<br/>其次，明确PPI的计算公式，根据博主Sebasiten Gabriel 叙述```DPI or Dots Per Inch is a measure of spatial dot density initially used in print. It's the number of ink drops your printer can put in an inch. The more dots per inch, the sharper your image.
This concept is applies to computer screens under the name PPI for Pixels Per Inch. Same principle: It counts the number of pixels your screen displays per inch. The name DPI is also used in screens.```， 假设`P` 是代表Pixels，`I`代表Inches，且`1Inch = 2.54cm`, 所以的表盘对角线的英寸是`Math.sqrt(Math.pow(21.22,2)+Math.pow(26.54,2))/25.4 = 1.3378`。根据Band Design Guide中的尺寸。得知42mm的Active Area为`30.42 * 24.66`，所有同理可得42mm的对角线尺寸是` = 1.54 ~ 1.5`，所以答案是*A和C*；对角线像素长度 = `Math.sqrt(Math.pow(340,2) + Math.pow(272,2)) = 435.4`，得到38mm的表屏幕尺寸为`435.4/`，计算高度方向的PPI,`P = 340px, I = 1.3378 `，所以得到`PPI = 435.4/1.3378 = 325.459 ~ 326 `。因为苹果官网上没有明确指出38mm和42mm的范围，导致很多人误解，以为是指Active Area区域的高度，所以有`290\302`这两种PPI。有些动手能力强的网友尝试自己用[游标卡尺测量](https://ooo.0o0.ooo/2016/08/30/57c57eb9c074b.jpg)，得出正确的结论。不过这个方法有点耿直。
</div>
1. Apple Watch如果没有配对的iPhone功能是有限的，如果需要iPhone配对，可采用蓝牙*Bluetooth 4.0*和Wi-Fi *(802.11b/g/n 2.4GHz）*两种方式来通讯，根据官网资料[About Bluetooth and Wi-Fi on Apple Watch](https://support.apple.com/en-hk/HT204562)所述，没有可连接WiFi时，Apple Watch和iPhone的链接是通过蓝牙来通讯的。阅读以上资料，假设使用环境为普通的室内办公环境，请选择Apple Watch和iPhone可正常的最远能相隔多远。（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
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
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是（C）试题解析**  
这个问题，可能没有标准答案。`Bluetooth uses radio waves (short-wavelength UHF to be exact) between 2.4 and 2.485 GHz in the ISM band. Long story short, that means that a Bluetooth signal can be interrupted by Wi-Fi signals, satellite dishes, certain external monitors, microwaves, bodies, certain electronics, etc.` ，所以在不同的环境下测试的结果可能不同，根据我自己的测试有效距离是30m，而其他人测试的结果可能是` up to 330 feet (100 meters) `，这个结论来自[What is the Apple Watch connection distance to iPhone?](http://bradymower.com/apple-watch-connection-distance-iphone/)，类似的讨论也有，比如这个讨论帖，[What's the farthest distance one can go before the Watch loses connection with the iPhone?](http://forums.imore.com/apple-watch/334781-what-s-farthest-distance-one-can-go-before-watch-loses-connection-iphone.html)。在翻阅了其他关于蓝牙有效距离的之后，发现如下结论:`有效距离和功率相关`，![](http://ooo.0o0.ooo/2016/09/13/57d76c66ba60d.jpg)`Officially Class 3 radios have a range of up to 1 metre (3 ft), Class 2, most commonly found in mobile devices, 10 metres (33 ft), and Class 1, primarily for industrial use cases,100 metres (300 ft).[3] Bluetooth Marketing qualifies that Class 1 range is in most cases 20–30 metres (66–98 ft), and Class 2 range 5–10 metres (16–33 ft).[2]`,而Apple Watch采用的是*Bluetooth 4.0*，根据表格![](http://ooo.0o0.ooo/2016/09/13/57d76cefbc865.jpg)可见应该最大是69m，而`Bluetooth Marketing qualifies that Class 1 range is in most cases 20–30 metres (66–98 ft)`，可侧面说明应该是30m左右。以上资料来自 wikipedia，[Bluetooth词条](https://en.wikipedia.org/wiki/Bluetooth#Setting_up_connections)。
</div>
1. 官方文档[App Programming Guide for watchOS](https://developer.apple.com/library/watchos/documentation/General/Conceptual/WatchKitProgrammingGuide/index.html)有以下描述，[Developing for Apple Watch](https://developer.apple.com/library/watchos/documentation/General/Conceptual/WatchKitProgrammingGuide/index.html#//apple_ref/doc/uid/TP40014969-CH8-SW1) 章节里`The projects you create for Apple Watch consist of two separate bundles: a Watch app and a WatchKit extension. The Watch app bundle contains the storyboards and resource files associated with all of your app’s user interfaces. The WatchKit extension bundle contains the extension delegate and the controllers for managing those interfaces and for responding to user interactions. While these bundles are distributed inside an iOS app, they are then installed on the user’s Apple Watch and run locally on the watch.`；[Configuring Your Xcode Project](https://developer.apple.com/library/watchos/documentation/General/Conceptual/WatchKitProgrammingGuide/ConfiguringYourXcodeProject.html#//apple_ref/doc/uid/TP40014969-CH2-SW1)章节中`You can either add a Watch app target to an existing iOS project, or create a new iOS project that includes a Watch app. In both cases, Xcode automatically configures the Watch app and WatchKit extension bundles and their initial resources. Those bundles are then delivered as part of your iOS app on the App Store.`；相同章节中也给出了Target structure in watchOS的结构图![](https://developer.apple.com/library/watchos/documentation/General/Conceptual/WatchKitProgrammingGuide/Art/target_structure_2x.png)，而在安装完毕之后，章节[The Watch App Architecture]()中展示了运行态的关系是![Relationship between the Watch app interface, the WatchKit extension, and the iOS app](https://developer.apple.com/library/watchos/documentation/General/Conceptual/WatchKitProgrammingGuide/Art/architecture_compared_2x.png)试阅读上述资料，回答以下问题。第一：在三个Target（iOS app, Watch app, WatchKit extionsion)的plist文件里都有一个字段`Bundle OS Type code`,试分别设置对应的值，iOS app =（ <input class="w-answer_inputer" type="text" name="answer"/> ），Watch app =（ <input class="w-answer_inputer" type="text" name="answer"/> ），WatchKit extionsion =（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	APPL
	</li>
	<li>
	FMWK
	</li>
	<li>
	BNDL
	</li>
	<li>
	XPC!
	</li>
</ol>
第二：结合题目1，假设Watch app因为加载了大图片，因为内存紧张而crash，问：iOS app会随着crash吗？（ <input class="w-answer_inputer" type="text" name="answer"/> ）；WatchKit extension会随着crash吗？（ <input class="w-answer_inputer" type="text" name="answer"/> ）。假设WatchKit extension里因为出现`1/0`的代码导致crash，问：iOS app会随着crash吗？（ <input class="w-answer_inputer" type="text" name="answer"/> ）；Watch app会随着crash吗？（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	是的，会跟着crash，因为在plist中配置了依赖关系
	</li>
	<li>
	不会crash，因为是3个不同Target，不会相互干扰
	</li>
	<li>
	我不知道，我也不想猜
	</li>
</ol>
第三：以网易有钱为例，最新版支持iOS10和WatchOS。假设Watch app + WatchKit extension的安装之后容量是20M，iOS app是30M，并且iOS app的`Deploy target`是iOS7以上。Watch app + WatchKit 配置的`Deployment target`都是3.0，问：某iPhone6用户升级到iOS10，但是没有配对的Apple Watch，此时从Apple store 下载的网易有钱安装包，安装之后是占用容量多大？（ <input class="w-answer_inputer" type="text" name="answer"/> ）；某iPhone6用户是iOS9，配对的Apple Watch是WatchOS 2，此时从Apple store 下载的网易有钱安装包，安装之后是占用容量是多大？（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	大约30M
	</li>
	<li>
	大约50M
	</li>
	<li>
	不能安装
	</li>
	<li>
	我不知道，我也不想猜
	</li>
</ol>
第四：接第三个问题上下文。某用户是iOS9，配对的Apple Watch是WatchOS 2，安装最新网易有钱，此时Apple Watch的网易有钱Watch app是如何表现？（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	因为版本不匹配，没有安装，所有Apple Watch上的网易有钱Watch app还是旧版本，但是不能正常工作，如crash等
	</li>
	<li>
	因为版本不匹配，卸载了旧版本的网易有钱Watch app
	</li>
	<li>
	在iPhone上的watch程序里 *我的手表*tab里，看到网易有钱的选项，点击进入安装，安装时，弹出`请升级watchOS`版本的提示
	</li>
	<li>
	因为版本不匹配，此用户不会收到可更新网易有钱iOS app的更新提示
	</li>
</ol>
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是：第一题目（A），（A），（D）；第二题目（B），（A），（B），（A）；第三题目：（B），（B）；第四题目：（B）试题解析**  
第一题目答案是（A），（A），（D）。回答这个问题之前需要搞清楚Bundle OS Type code，官方文档里[CFBundlePackageType](https://developer.apple.com/library/mac/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html#//apple_ref/doc/uid/20001431-111321) 部分提到`CFBundlePackageType (String - iOS, OS X) identifies the type of the bundle and is analogous to the Mac OS 9 file type code. The value for this key consists of a four-letter code. The type code for apps is APPL; for frameworks, it is FMWK; for loadable bundles, it is BNDL. For loadable bundles, you can also choose a type code that is more specific than BNDL if you want.
All bundles should provide this key. However, if this key is not specified, the bundle routines use the bundle extension to determine the type, falling back to the BNDL type if the bundle extension is not recognized.`。此字段是Mac OS的遗产，在iOS端，打包时做校验，缺少或者错误设置可能导致无法submit app，例如[Techincal Q&A QA1273](https://developer.apple.com/library/ios/qa/qa1273/_index.html)。经过测试，这个字段在Debug模式下是无所谓什么值。*APPL*表明是一个独立的APP，而*XPC！*表明是XPC Services服务。之所以苹果将WatchKit extension设计为XPC服务，为了减少对其它Target的影响。`XPC services are managed by launchd, which launches them on demand, restarts them if they crash, and terminates them (by sending SIGKILL) when they are idle. This is transparent to the application using the service, except for the case of a service that crashes while processing a message that requires a response. In that case, the application can see that its XPC connection has become invalid until the service is restarted by launchd. Because an XPC service can be terminated suddenly at any time, it must be designed to hold on to minimal state—ideally, your service should be completely stateless, although this is not always possible.` 。[Understanding the Structure and Behaviour](https://developer.apple.com/library/mac/documentation/MacOSX/Conceptual/BPSystemStartup/Chapters/CreatingXPCServices.html#//apple_ref/doc/uid/10000172i-SW6-SW1)。<br/> 在实际测试中发现，Watch app和WatchKit extension是耦合的，要崩溃一起奔溃，两者崩溃时对iOS app没有影响，第二个题目的答案是B），（A），（B），（A）————是不是很简单的答案？然而看到XPC server这种服务的时候，很好奇 3个Target（iOS app, Watch app, WatchKit extionsion)是如何组织在一起的。从代码层面得到结论：iOS app的`Build Phases`里添加了Watch app为`Target Dependecies`之一，同时Watch app的plist里字段`WKCompanionAppBundleIdentifier`是iOS app的bundleId，而WatchKit app的plist的`WKAppBundleIdentifier`字段则是Watch app的bundleID，是这样连一起的。在文件系统中，是3层的包含关系。在安装包里的结构是`ipa > iOS app > Watch/ > Watch app > Plugins/ > WatchKit extension.appex` ，但是运行时的结构却是`/var/containers/Bundle/Application/ > iOS app `和`/var/containers/Bundle/Application/ > Watch.app > PlugIns > appleWatch Extension.appex`，可见iOS app和Watch app是平级的应用，相互之间通讯的方式受此条件限制。
<br/>
不同iOS设备、不同iOS版本安装包的容量本身就不一样，安装之后的容量也是不一样的。以网易有钱2.5.0.1411而言。分别在iOS8.4和iOS10上的appstore里搜索`网易有钱`， <br/>
<a class="w-view_img" href="https://ooo.0o0.ooo/2016/10/17/58049581895f7.png" target="_blank">
		<img title="iOS10的appstore" style="width:300px;" src="https://ooo.0o0.ooo/2016/10/17/58049581895f7.png"/>
	</a>，可见在iOS10上，安装包是43.3M，而实际上安装完毕之后，占用磁盘的容量却是39.3M；<br/>
	<a class="w-view_img" href="https://ooo.0o0.ooo/2016/10/17/5804958189c80.png" target="_blank">
		<img title="iOS8.4的appstore" style="width:300px;" src="https://ooo.0o0.ooo/2016/10/17/5804958189c80.png"/> 
	</a>，
	而在iOS10上安装包是是40.7M，安装完毕之后占用磁盘容量是53.7M。经过在iPhone5、iPhone6、iPhone6PiOS10设备上的测试，他们的安装包和安装后的占用容量都是一样的；同时iOS8的iPod和iPhone5安装包和安装后的占用容量都是一样的———和是否有Apple Watch配对无关，这样某设备一旦检测有Apple Watch配对，可以本地将iOS上搭载的Watch app安装到Apple Watch上，所以第三题目都是（B），（B）。因为用户是iOS9，大于部署的目标版本，所以iOS app是可以更新的，而iPhone配对的Apple Watch的watchOS版本不符合`Deploy target`，watchOS3是没有bundled在iOS9的设备上，所以在iPhone上的`Watch` app里不会显示对应Watch app，如果是旧版本有Watch app，则会卸载掉就版本的Watch app。第四题目，答案是（B）
</div>
1. 根据App Programming Guide for watchOS 章节[Communicating with Your Companion iOS App](https://developer.apple.com/library/watchos/documentation/General/Conceptual/WatchKitProgrammingGuide/SharingData.html#//apple_ref/doc/uid/TP40014969-CH29-SW1), `Use the Watch Connectivity framework to communicate between your WatchKit extension and iOS app. That framework provides bidirectional communications between the two processes and lets you transfer data and files in the foreground or background.`，一共有4组，分别是`updateApplicationContext:error:`，`transferUserInfo:和
transferCurrentComplicationUserInfo:`，`transferFile:metadata:`，`sendMessage:replyHandler:errorHandler:和sendMessageData:replyHandler:errorHandler:`，试根据以上资料，判断以下描述哪些是正确的？（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	以上接口大概分为两种传输方式，一种是background 一种是foreground。支持后台传输的有`updateApplicationContext:error:`，`transferUserInfo:和transferCurrentComplicationUserInfo:`，`transferFile:metadata:`；支持前台传输的是`sendMessage:replyHandler:errorHandler:和sendMessageData:replyHandler:errorHandler:`。
	</li>
	<li>
	以上接口，WatchKit extension和iOS app之前传输速度排行 `sendMessage:replyHandler:errorHandler:和sendMessageData:replyHandler:errorHandler:` >= `transferCurrentComplicationUserInfo:` > `transferUserInfo:和updateApplicationContext:error:` > `transferFile:metadata:`
	</li>
	<li>
	以上接口中，只有`sendMessage:replyHandler:errorHandler:和sendMessageData:replyHandler:errorHandler:`可以从WatchKit extension端唤醒iOS app，并立即*及时*调用iOS app的相关接口。而iOS app没有办法唤醒WatchKit extension，并且立即执行WatchKit extension相关接口，只有等待watchOS系统自身在合适的时机在后台或者前台传输数组，也就是说依赖iOS app端发起数据传输是不可靠的。根据此特征，在watchOS日常业务开发中，我们采用从WatchKit extension端发起数据请求，iOS响应、返回数据的方式；而iOS app向WatchKit extension发起数据传输，作为为WatchKit extension做数据缓存的补充手段。
	</li>
	<li>
	以上接口中，当iOS app调用`sendMessage:replyHandler:errorHandler:和sendMessageData:replyHandler:errorHandler:`之后，如果在等待replayhandler被调用返回的过程中，Apple Watch和iPhone之间disconnect，那么在reconnect之前，请求返回值调用会被丢弃；而当iOS app调用`transferUserInfo:和updateApplicationContext:error:`之后，本次请求没有即时发送到Apple Watch，之后双方disconnect，过一段时间之后重新reconnect，则会继续在合适的时间发送数据到Apple Watch；而当iOS app调用`transferUserInfo:和updateApplicationContext:error:`之后，本次请求没有即时发送到Apple Watch，之后iOS app或者Watch app被kill，那么此次传输数据被丢失，iOS app或者Watch app在重启之后 也不会继续传输。
	</li>
	<li>
	以上接口中，`sendMessage:replyHandler:errorHandler:和sendMessageData:replyHandler:errorHandler:`的传输只有在iOS app向WatchKit extension发送时，需要reachable==YES的情况下请求；而WatchKit extension向iOS app请求时则不需要reachable==YES成立。
	</li>
</ol>
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是（A，B，E）试题解析**  
答案C，根据文档`transferCurrentComplicationUserInfo: method to send complication-related data from your iOS app to your Watch app. This method sends a high priority message to your WatchKit extension, waking it up as needed to deliver the data and update the complication’s timeline.
Be aware, however, that your complication has a limited daily budget for updates. ` 可知`transferCurrentComplicationUserInfo:`拥有较高的传输优先级，而且可以唤醒WatchKit extension。答案C其余部分表述是正确；答案D，`updateApplicationContext:error:`会将需要传输的数据 存档archive为文件，保存到沙盒，所以即使kill掉Watch app被kill掉，沙盒文件不会别删除，所以还是处于待传输状态。
</div>
1. 接上述题目，以典型的`updateApplicationContext:error:`代表后台传输，以`sendMessage:replyHandler:errorHandler:`代表前台（或者称之立即传输），假设WatchKit没有效率、电量、其他数据排队的因素考虑的情况下，请判断下述情况下，执行上述代码后（以上代码均在iPhone端执行），数据的传输情况。<br/>第一：当iOS app处于前台、Apple Watch处于前台,执行后（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app可以使用数据
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app可以使用数据
	</li>
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新进入主界面
	</li>
</ol>
第二：当iOS app处于前台、Apple Watch处于点亮状态，Watch app刚刚切换到后台期间,执行后（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app可以使用数据
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app可以使用数据
	</li>
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新进入主界面
	</li>
</ol>
第三：当iOS app处于前台、Apple Watch处于点亮状态，Watch app切换到后台期间有一段时间了,执行后（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`updateApplicationContext:error:`数据尚未传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据尚未传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`updateApplicationContext:error:`数据尚未传输到Apple Watch，本次数据丢失，即使Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据尚未传输到Apple Watch，本次数据丢失，即使Watch app重新启动进入主界面</li>
</ol>
第四：当iOS app处于前台、而Watch app被kill掉，Apple Watch屏幕处于熄灭状态,执行后（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`updateApplicationContext:error:`数据尚未传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据尚未传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
</ol>
第五：同题目三，但是此Watch app被设置为`Keep In Dock`当iOS app处于前台、Apple Watch处于点亮状态，Watch app切换到后台期间有一段时间了,执行后（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	`updateApplicationContext:error:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据已经传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`updateApplicationContext:error:`数据尚未传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据尚未传输到Apple Watch，Watch app不可以使用数据，直到Watch app重新启动进入主界面
	</li>
	<li>
	`updateApplicationContext:error:`数据尚未传输到Apple Watch，本次数据丢失，即使Watch app重新启动进入主界面
	</li>
	<li>
	`sendMessage:replyHandler:errorHandler:`数据尚未传输到Apple Watch，本次数据丢失，即使Watch app重新启动进入主界面</li>
</ol>
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是 第一题（A，B），第二题（A，B），第三题C,F），第四题（C），第五题（C,F）试题解析**
回答这个问题之前，需要熟悉Watch app的生命周期。
对于Watch app而言，一共会有5个状态。其中suspend是非常短时间的一个状态。这时候的Watch app运行在background模式，此后只有workout可以继续运行，其他的一律停止运行，参见[WKBackgroundModes](https://developer.apple.com/library/prerelease/content/documentation/General/Reference/InfoPlistKeyReference/Articles/watchOSKeys.html#//apple_ref/doc/uid/TP40016498-SW8)。设置为保留在Dock只是处于Suspend状态，`The app is in memory but is not executing code. The system suspends apps that are in the background and do not have any pending tasks to complete. The system may purge suspended apps at any time to make room for other apps. The system silently purges suspended apps. The suspended apps do not wake, and do not receive any notifications before being purged.`
</div>
1. 在watchOS 3中，提供了一个新的接口 `WKExtension scheduleBackgroundRefreshWithPreferredDate:userInfo:scheduledCompletion:`，Schedules a background task to refresh your app’s data，请问以下方式哪种方法，可以取消已经生效的定时任务。（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>
	使用相同参数设置定时任务，可取消上一次定时任务
	</li>
	<li>
	kill掉Watch app
	</li>
	<li>
	卸载Watch app，之后重新安装
	</li>
	<li>
	删除沙盒文件系统中的Library和Document文件
	</li>
</ol>
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是（A，C）试题解析**  
在文档中[1650848-schedulebackgroundrefreshwithpre](https://developer.apple.com/reference/watchkit/wkextension/1650848-schedulebackgroundrefreshwithpre?language=objc)和watchOS API里，特别的注释了`// there can only be one background refresh request at any given time. Scheduling a second request will cancel the previously scheduled request`。后台任务只能有一个，这个限制不太符合业务需求；还有一个限制——在complication里做动画，也会受限于reloadComplication budget（据说是一天只有50次机会）。这让实现功能的时候很掣肘，鸡肋的API，鸡肋的设计。<br/>B, 文档中提到`Call this method to update the contents of your app in the background. When the task is triggered, the system wakes your app in the background and calls your extension delegate’s handleBackgroundTasks: method. `，是可以唤醒app，所以被kill掉也会被重启，所以B错误。<br/>答案C，实际测试是可以取消的，猜测卸载Watch app时会清理掉相关定时任务。<br/>答案D，不像`updateApplicationContext:error:`保存到iOS app的内容沙盒中，`scheduleBackgroundRefreshWithPreferredDate:userInfo:scheduledCompletion`注册到watchOS 系统内部来实现定时任务，类似launchd管理，在沙盒里没找到和定时任务有关系的文件。
</div>
1. 从iOS (9.0 and later)开始，`WCSession`有一个属性`watchDirectoryURL`,根据API的注释`Use this directory to persist any data specific to the selected Watch. The location of the URL will change when the selected Watch changes. This directory will be deleted upon next launch if the watch app is uninstalled for the selected Watch, or that Watch is unpaired. If the watch app is not installed for the selected Watch the value will be nil.`。文档[WCSession]() `Your iOS app can use the watchDirectoryURL property to store data that is specific to only one instance of your Watch app running on a particular Apple Watch. In most cases, the data you display in each instance of your Watch app is the same. However, you might use this directory to store configuration data, preferences, or other data files that your iOS app needs to interact properly with your Watch app. If you do, use the activation and deactivation process to update your iOS app`。通常用来作为要传输到WatchKit extension端文件的缓存地点，作用类似macOS上的`~`目录，方便管理。如贴文[iOS-WatchKit File Transfers Work Unreliably](http://stackoverflow.com/questions/34477577/ios-watchkit-file-transfers-work-unreliably)。根据上述表述，试确定`watchDirectoryURL`的绝对目录，（****）表示随机字符的文件夹
（ <input class="w-answer_inputer" type="text" name="answer"/> ）
<ol class="innerList" type="A">
	<li>`/var/mobile/Containers/Data/Application/****/Library/Application%20Support/com.apple.watchconnectivity/****/WatchContent/****/`</li>
	<li>`/var/mobile/Containers/Data/Application/****/Documents/Inbox/com.apple.watchconnectivity/****/WatchContent/****/`</li>
	<li>`/var/containers/Bundle/Application/****/Library/Application%20Support/com.apple.watchconnectivity/****/WatchContent/****/`</li>
	<li>`/var/containers/Bundle/Application/****/Documents/Inbox/com.apple.watchconnectivity/****/WatchContent/****/`</li>
</ol>
<button type="submit" class="w-open-answer" name="viewAnswer" onclick="var ele = this.nextElementSibling;ele.style.display = (ele.style.display=='none'?'block':'none');">查看答案</button>
<div class="w-answer-content" style="display:none">
**答案是（A）试题解析**  
这个答案包含了一系列的知识点，[About the iOS File System](https://developer.apple.com/library/content/documentation/FileManagement/Conceptual/FileSystemProgrammingGuide/FileSystemOverview/FileSystemOverview.html)。<br/>一，普通iOS app的在安装之后，有两块区域，一块是BundleContainer，一块是Data Container，二者在不同的目录，但是共同属于iOS app的Sandbox；`For security purposes, an iOS app’s interactions with the file system are limited to the directories inside the app’s sandbox directory. During installation of a new app, the installer creates a number of container directories for the app inside the sandbox directory. Each container directory has a specific role. The bundle container directory holds the app’s bundle, whereas the data container directory holds data for both the app and the user. The data container directory is further divided into a number of subdirectories that the app can use to sort and organize its data. The app may also request access to additional container directories—for example, the iCloud container—at runtime.`见图<a class="w-view_img" href="https://developer.apple.com/library/content/documentation/FileManagement/Conceptual/FileSystemProgrammingGuide/art/ios_app_layout_2x.png" target="_blank">
		<img title="An iOS app operating within its own sandbox directory" style="width:300px;" src="https://developer.apple.com/library/content/documentation/FileManagement/Conceptual/FileSystemProgrammingGuide/art/ios_app_layout_2x.png"/>
	</a>。所以，在运行时检查`[[NSBundle mainBundle] bundlePath]`，输出形如`/var/containers/Bundle/Application/7D3CCF0B-4422-406F-A0D8-1A830D312481/MoneyKeeper.app`的目录；而`[NSSearchPathForDirectoriesInDomains(NSDocumentDirectory, NSUserDomainMask, YES) firstObject]`，输出形如`/var/mobile/Containers/Data/Application/3B2429B5-A779-4FC3-9C11-05542B47AB43/Documents`的目录。而可读写的区域是`Bundle Container`,所以排除掉答案`C,D`。至于是`Application Support`还是`Inbox`，可以查阅官方文档中的描述，其中针对`Documents/Inbox`的的说明是，`Use this directory to access files that your app was asked to open by outside entities. Specifically, the Mail program places email attachments associated with your app in this directory. Document interaction controllers may also place files in it.
Your app can read and delete files in this directory but cannot create new files or write to existing files. If the user tries to edit a file in this directory, your app must silently move it out of the directory before making any changes.
The contents of this directory are backed up by iTunes and iCloud.`，而针对`Application Support`的说明[The Library Directory Stores App-Specific Files](https://developer.apple.com/library/content/documentation/FileManagement/Conceptual/FileSystemProgrammingGuide/FileSystemOverview/FileSystemOverview.html#//apple_ref/doc/uid/TP40010672-CH2-SW1)是`Use this directory to store all app data files except those associated with the user’s documents. For example, you might use this directory to store app-created data files, configuration files, templates, or other fixed or modifiable resources that are managed by the app. An app might use this directory to store a modifiable copy of resources contained initially in the app’s bundle. A game might use this directory to store new levels purchased by the user and downloaded from a server.
All content in this directory should be placed in a custom subdirectory whose name is that of your app’s bundle identifier or your company.
In iOS, the contents of this directory are backed up by iTunes and iCloud.`。总结一下,`Application Support`里保存的是程序本身运行时需要的文件，而`Documents/Inbox`里的文件可能和外部程序通讯时使用，而且是可被用户看到的。所以是答案A。实际测试也证实如此，你也能发现`Library/Preferences`文件下包含一个app bundleId.plist文件，Userdefault的数据就被持久化在这个文件里。在这些目录中，也有Inbox和Application Support这样的目录，这些目录是来保存异步消息文件的地方。如`updateApplicationContext:error:`是通过将消息，通过archive的方式（经过观察各个文件的内容格式，类似是archive之后的内容。有些文件的内容又指向另外一个plist文件，猜测是archive持久化）保存到iOS app的内容沙盒中，
</div>

<input type="button" value="我答完了" name="finish" id="finish"/> &nbsp;总得分<span style="color:red;font-size:18px;" id="score"></span>  &nbsp;<a id="viewAnswerLink" style="display:none;" href="/demo.html?viewAnswer=true">查看题目解析</a>


