## 1:1 模式

人脸验证做的是1:1的比对，其身份验证模式本质上是计算机对当前人脸与人像数据库进行快速人脸比对，并得出是否匹配的过程，
可以简单理解为证明你就是你。

1:1作为一种静态比对，一般在金融、信息安全领域中应用较多。例如在机场、高铁站安检时，受检人员手持身份证等证件，
通过检查通道，同时对受检人员的外貌及身份证信息进行识别，此过程就是典型的1:1模式的人脸识别。


## 1:N 模式

人脸识别做的是1:N的比对，即系统采集了“我”的一张照片之后，从海量的人像数据库中找到与当前使用者人脸数据相符合的图像，
并进行匹配，找出来“我是谁”。

1:N人脸识别模式，同时具有动态比对与非配合两种特点。动态对比是指通过对动态视频流的截取来获得人脸数据并进一步比对的过程；
而非配合性是指识别的过程表现出非强制性与高效性的特点，识别对象无需到特定的位置便能完成人脸识别的工作。



## M:N 模式

M:N 是通过计算机对场景内所有人进行面部识别并与人像数据库进行比对的过程。M:N作为一种动态人脸比对，其使用率非常高，
能充分应用于多种场景，例如公安布控等。

M:N模式难度和要求较大，因为其必须依靠海量的人脸数据库才能运行，并且由于识别基数大，图像采集设备受环境影响等因素，
使M:N模式可能产生较高的错误率从而影响识别结果。

















------------------------以下为老版本重构前的LOG----------------------------------
# V1.0.0

  - 工程建立，环境搭建
  

# V1.0.0 Alpha01

  - 添加人脸检测，人脸识别
  - 活体检测 初版


# V1.0.0 Alpha02

  - 添加超时检测
  - 修复闪退问题

# V1.0.0 Beta03

 - 支持自定义 Threshold（阈值）
 - 修复快速返回后的Bad Token 问题
 - 高仿微信人脸识别UI样式


# V1.1.0
 - 优化使用体验
 - 加快检测速度
 

# V2.0.0
- 添加1：N 检验


# V3.0.0
- 重构使用方式，简化接入步骤
- 完善极端情况操作，提高稳健性
- 

# V3.3.0
- 提高安全性，人脸数据私有目录保持
- 重构使用方式，简化接入步骤


# V3.5.0
- 活体检测倒计时动画

# V3.7.0
- 提高人脸识别预览成像质量
- 活体检测防止照片攻击
- 优化识别过程用户体验问题
- 支持Android 5-13，Target SDK=33

# V3.7.3
- 提高中高端设备识别精确度，低配设备时间换效率吧
- 优化动作活体检测的完整性

# V3.8.0
- 添加静默活体检测，防止视频合成等欺骗
- 修复超时重试动作活体提示不准确问题

# V3.7.3
- 提高中高端设备识别精确度，低配设备时间换效率吧
- 优化动作活体检测的完整性

# V3.8.0
- 添加静默活体检测，防止视频合成等欺骗
- 修复超时重试动作活体提示不准确问题

# V3.9.0

- 支持平板横屏幕
- 1：N 识别迁移独立支持N大于1000离线快速检索