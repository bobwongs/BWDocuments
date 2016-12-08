# iOS项目开发经验之开发资源和开发配置

开发iOS项目所需要的开发资源和开发配置

## Contents

- 开发配置
- 开发资源
- 第三方开发库
- 开放平台
- 证书和Apple开发账号
- 应用上线
- Follow Me

## 开发配置

> Create An iOS Xcode Project

图示

说明

Single View Application：新建Xcode项目的模板名称
Team：开发者账号
Product Name：Xcode项目名称
Organization Name：组织名称
Organization Identifier：组织标识
Language：开发语言，Objective-C or Swift
Devices：开发的目标设备，iPhone, iPad, Universal
Use Core Data：是否使用Core Data
Include Unit Tests：是否包含单元测试
Include UI Tests：是否包含UI测试

> Info.plist

Bundle Identifier
Display Name：App的显示名称
Version(Bundle versions string, short)：项目版本
Build：项目Build号
Deployment Target：项目最低兼容到的iOS系统版本
Device Orientation：设备支持的屏幕显示方向

> Capabilities

所具备的能力，由Apple提供的功能；

> Build Settings

Architectures
Signing
​	Code Signing Identity
​	Provisioning Profile
Apple LLVM - Language
​	Prefix Header
Apple LLVM - Preprocessing
​	Preprocessor Macros

> Build Phases

Compile Sources
Link Binary With Libraries
Copy Bundle Resources

> Assets.xcassets

见开发资源

## 开发资源

> Assets.xcassets

**AppIcon**
尺寸，分别需要2x和3x的，即2倍图和3倍图，如20.0，需要40×40和60×60的图
20.0: iPhone Notification iOS 7-10 20pt
29.0: iPhone Spotlight - iOS 5,6 Settings - iOS 5-10 29pt
40.0: iPhone Spotlight iOS 7-10 40pt
60.0: iPhone App iOS 7-10 60pt
**LaunchImage**
iPhone Portrait iOS 8,9
Retina HD 5.5’’, Retina HD 4.7'’
iPhone Portrait iOS 7-9
2x, Retina 4

## 第三方开发库

> 管理工具

CocoaPods

> Library

AFNetworking
Masonry
IQKeyboard
SDWebImage
MJExtension
MJRefresh
MBProgressHUD
SVProgressHUD
YYCategories

## 开放平台

微信；
支付宝；
微博；
银联；
友盟；
个推；
百度地图；
高德地图；

## 证书和Apple开发账号

参考《iOS 项目经验之证书和Apple开发账号》，链接：之后补上

## 应用上线

> 应用管理平台

Apple官方网址
​	https://itunesconnect.apple.com/
账号
​	Apple ID

> 新建iOS App Store App

基本信息
​	名称
​		App 在 App Store 中显示的名称；
​	主要语言
​		如果 App 信息没有针对某个国家的 App Store 进行本地化, App 信息将以主要语言呈现；
​	套装 ID
​		Bundle ID；
​	版本
​		版本号会显示在 App Store 中，并且应与您在 Xcode 中所使用的版本号相符；
​	SKU
​		一个独特的、不会在 App Store 中显示的 App ID；
版本信息
​	App 视频预览和屏幕快照
​		屏幕快照必须为 JPG 或 PNG 格式，且必须采用 RGB 颜色空间。 App 视频预览必须为 M4V、MP4 或MOV 格式，且不能超过 500 MB；
​	描述
​		对您 App 的描述，用以详细说明特性和功能；
​	关键词
​		一个或多个关键词，用以描述您的 App。关键词将使 App Store 搜索结果更加准确。关键词之间用英文逗点分隔；
​	技术支持网址(URL)
​		您的 App 技术支持网址(URL)。该网址将会在 App Store 中显示；
​	营销网址(URL)
​		您的 App 营销信息网址(URL)。该网址会在 App Store 中显示；
​	隐私政策网址(URL)（可不填）
​		您所在机构的隐私政策网址(URL)。面向儿童的、提供自动续费的 App 内购买项目、及免费订阅的 App, 均需隐私政策。另外, 需用账户注册的、或用现有账户进入的、以及有法律另行规定的 App 也需隐私政策。对于收集用户或设备相关数据的 App, 亦推荐使用隐私政策；
App综合信息
​	App 图标
​		此图标将用于 App Store，其格式必须为 JPG 或 PNG，最低分辨率至少为 72 DPI，并采用 RGB 色彩空间。它不能包含图层或圆角；尺寸为1024×1024；
​	Apple ID
​		为您的 App 自动生成的 ID；
​	版本
​		您要填入的 App 版本号。编号应遵循软件版本规范；
​		注意：每次提交审核的版本号都是不同的，包括Xcode中的版本，要遵循版本规范；例如：这次提交的是1.0.0，那么下次需要提交的则是1.0.1，以此类推；
​	类别
​		最能准确描述此 App 的类别。有关更多信息；
​	评级

​	版权
​		拥有您的 App 专有权的人员或实体的名称，前面是获得权利的年份（例如“2008 Acme Inc”）；
构建版本
​	通过Xcode提交；
App 审核信息
​	联系信息；
版本发布
​	自动发布；
​	手动发布；

> 定价

定价格

> App Store发布

注意Provisioning Profile的选择；

> 企业证书发布

直接进行企业分发

> 加急审核

描述
​	由于某些原因，需要加快应用的审核进程，可以通过发邮件的方式给Apple来加急审核；
网站
​	https://developer.apple.com/contact/app-store/?topic=expedite
Apple收到加急审核
​	We've received your request.
心得
​	在需要用到加急的时候都可以发邮件给Apple，当然加急审核也要适度使用；
​	提高英文描述的能力，锻炼自己的英文，虽然也可以用中文来描述原因，做好描述原因的文档记录。

## Follow Me

Github: https://github.com/bobwongs