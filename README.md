各个部分的界面如下：

​                                ![电脑萤幕画面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image002.png)

图2-3-27 系统入口

![图形用户界面, 网站  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image004.png)

图2-3-28 服务介绍

![图形用户界面, 网站  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image006.png)

图2-3-29 支持品牌

![图形用户界面, 应用程序  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image008.png)

图2-3-30 项目特色

![图形用户界面, 应用程序  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image010.png)

图2-3-31联系方式

(1)   固件上传界面

固件上传界面包括上传二进制固件，设置固件名称，选择固件品牌和进行固件描述。这些固件信息将提供给之后的仿真模拟。

![图形用户界面, 应用程序  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image012.png)

图2-3-32 固件上传页面

在固件上传过程中，将对固件的文件类型进行过滤，只允许上传.bin文件或压缩格式的文件，否则页面将会出现错误，如下：

![图形用户界面, 文本, 应用程序, 电子邮件  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image014.png)![图形用户界面, 应用程序  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image016.png)

图2-3-33 上传格式错误

(2)   容器集群管理界面

容器集群管理功能主要为容器数据展示和容器管理。

![img](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image018.png)

图2-3-34 固件容器集群管理界面

具体而言，在数据展示部分，用户可从页面上方可以了解到历史测试的固件数量和正在当前正在测试的固件数量，以及测试固件容器在Running，Stopped，Paused，Waited不同状态下的数量。同时用户可以通过页面上方右侧的动态网络拓扑图中了解到当前Running或Paused的固件的所在的网络环境和网络地址。

![图形用户界面, 应用程序  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image020.jpg)

图2-3-35 当前固件运行状态监测与网络拓扑展示

在页面右侧，平台可视化展现出了历史固件漏洞挖掘的统计结果，方便用户对测试集群的漏洞类型进行感知。在页面的底部，平台对历史固件的固件名称，固件类型，固件品牌，固件架构，测试崩溃次数进行展示，同时用户可以通过右侧下载按钮下载之前测试中产生的崩溃用例。

![图片包含 图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image022.jpg)

图2-3-36 历史固件测试统计数据展示

在容器生命周期管理部分，平台为用户提供了控制固件容器的操作接口，实现虚拟设备的创建，启动，停止，暂存等操作，同时后台的访问控制列表规范了用户对不同状态下的容器操作行为。如图所示，当用户需要对上传固件进行操作时，用户可以在容器集群管理界面中的固件控制板，点击固件容器中的相应的容器操作按钮。

![img](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image024.jpg)

图2-3-37 固件控制板

比如ID：003固件为刚刚上传的固件，目前的状态为Waiting，那么现在就可以对固件进行启动或者删除操作。同时点击获取按钮用户可以从下拉列表中对固件基本信息进行提取，或下载固件中的文件系统和内核。

![img](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image026.jpg)

图2-3-38 固件静态分析操作

(3)   终端交互界面

进入分控台后，首先是固件基本信息显示页面，左侧信息包括固件品牌、固件CPU架构、固件型号、服务器类型等。右侧提供固件系统信息，包括内核引导程序路径、内核版本号、文件系统hash值、文件系统类型和端口服务。用户可以在此页面获取固件的基本信息。

进入分控台后，可以选择页面上方的固件终端交互界面。点击导航栏后浏览器弹出提醒，点击确定后可进入固件的命令行界面中。

![img](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image028.jpg)

图2-3-39 弹出提醒及固件基本信息页面

在固件交互终端中，可以进入搭建好的python环境并运行程序文件，对固件环境进行网络监控、系统调试、端口扫描等，提供给用户实时监控固件系统运行状态的功能。

![img](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image030.png)

图2-3-40 终端控制界面

(4)   网络爬虫监控界面

网络爬虫监控界面包括模拟用户与浏览器的交互过程和捕获交互过程产生的数据包用以后续的解析树生成。

![图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image032.jpg)

![图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image033.jpg)

图2-3-41 网络爬虫监控界面

页面上方是自动化测试页面和嗅探器的状态信息，自动化测试页面指模拟用户与浏览器的交互过程，即输入帐号密码信息登录系统，并点击所有页面中可交互的控件。本系统可以在页面上方显示自动化测试页面是否完成和嗅探器的状态信息。

![图形用户界面, 应用程序  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image035.png)![图形用户界面, 网站  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image037.png)

图2-3-42 状态栏

爬虫控制台输出指在模拟用户与浏览器进行交互，嗅探器捕获数据包时终端产生的输出信息，包括模拟器的启动信息，点击控件类型，跳转页面以及嗅探器运行时信息等，方便用户更好地对网络爬虫过程进行监控。

 

![文本  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image039.png)

图2-3-43 爬虫控制台输出

在控制台输出右侧是爬虫自动化测试相关历史数据和交互数据包捕获相关历史数据。爬虫自动化测试相关历史数据提供了已测试页面个数、已交互控件个数、待爬取页面个数和已测试时间，方便用户跟踪自动化测试的进度，提供简单的统计信息。

![表格  中度可信度描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image041.png)![图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image043.png)

图2-3-44 相关统计信息

交互数据包捕获相关历史数据包括已捕获交互数据包总数、请求包个数、非静态资源请求包个数和已监听时间，用户可以实时监控数据包的捕获信息，了解嗅探器的工作状态和数据包的统计信息。

页面底部显示了已测试的可交互控件信息，包括序号、标签XPath定位、所属页面、标签类型和是否成功交互判断，用户可以通过查看可交互控件信息，获得更多固件运行信息，了解自动化测试总流程。

![图形用户界面, 应用程序, Teams  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image045.png)

图2-3-45 可交互控件信息

(5)   模糊测试界面

通过点击分控台上方的导航栏“模糊测试”，可以进入模糊测试界面。在该界面可查看有关模糊测试的相关信息，包括模糊测试进度、当前测试状态、测试时长、测试用例、当前页面字段评分、Crash记录、会话图、解析树等，提供给用户具体直观的模糊测试信息，且支持用户控制模糊测试进程，可暂停或重启，如图2-3-46所示。

![图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image047.jpg)

![图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image048.jpg)

图2-3-46 模糊测试页面

首先是模糊测试的控制台部分，可以查看当前页面总共要发送的测试用例个数、测试进度、运行时间、执行速度和当前测试的字段名等，向用户实时提供模糊测试的进度信息。

![文本  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image050.png)

图2-3-47 模糊测试控制台

控制台右边显示了节点平均fuzz次数、固件版本信息和测试时长，用户可对整个模糊测试过程所花费的时间进行估算，如下图所示。

![图形用户界面  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image052.png)

图2-3-48 fuzz信息

除此之外，本页面提供了模糊测试过程的详细信息，将命令行的输出显示在前端界面，其中包括发送报文长度，报文内容，固件是否成功响应等，有命令行和表格两种显示方式，为用户提供更详细的测试信息。

![文本  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image054.jpg)![图形用户界面, 表格  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image056.jpg)

图2-3-49 模糊测试详细信息

详细信息右侧显示了当前页面字段的三个漏洞维度评分，以玫瑰图的方式呈现，可以直观地了解各个字段的危险程度，将模糊测试功能过程化、具体化。

![图表, 雷达图  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image058.png)![表格  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image060.png)

图2-3-50 字段评分

下方显示了模糊测试过程产生的crash记录，包括crash产生的所在目标文件、请求节点、变异字段、变异结果和监控反馈，提供了详细的crash说明。 

![图形用户界面, 应用程序, Teams  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image062.png)

图2-3-51 Crash记录

页面最下方显示会话图和解析树，会话图将请求报文作为节点，其中红色节点代表当前测试点，灰色节点代表未测试点，绿色节点是登录点，上方显示模糊测试进度，可以使用户了解模糊测试的整个会话流程。解析树组将当前页面的可测试字段用树图的方式显示在前端页面中，有MsgTree和ETree两种显示方式，如下图所示2-3-52和图2-3-53所示。在会话图和解析树组的右上方都有下载功能选项，用户可以将其导出，方便分析，至此完成模糊测试监控。

![图片包含 图示  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image064.png)

图2-3-52 会话图和解析树组

![图示  描述已自动生成](https://github.com/dalision/Bamboofuzz/blob/main/images/clip_image066.png)

图 ETree-解析树组

 