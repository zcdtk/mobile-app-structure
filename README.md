# iBiz 移动端结构需求说明

信息技术发展到今天，作为信息的载体，移动端已经是必不可少的内容结构之一。

快速开发移动端，迭代能力

移动端，信息信息载体。

快速开发

快速迭代

模型化结构。

## 技术选型

基于 JavaScript 的小程序

H5 独立程序应用

三大框架的技术支持，Angular、React、Vue。



## 程序

移动端程序，



### 钉钉移动端结构说明

钉钉作为一个沟通平台，其移动端具备基本结构独立的常规功能和附加和，如注册登录等

#### 功能页面

##### 注册

<img src="imgs/function-page/register.jpg" alt="注册页面" style="zoom: 25%;" />

注册页面，是 app  的起点，打开 app 的第一步，就是注册用户信息，用户注册最简单方式，使用手机号码注册即可。另外，还可以使用邮箱注册、第三方授权注册等方式。

##### 登录

<img src="imgs/function-page/login.jpg" alt="登录" style="zoom: 25%;" />

登录页面，是 app 的入口，一般在独立的 H5 app 中，回出现登录页面。作为内容被集成到其他的应用应用中，会被应用应用授权，直接使用该应用用户信息；还有不需要登录，用户可以直接访问的页面，这个步骤会被省略。

app 登录方式与用户的注册方式，切实相关。如上图所示，用户可以使用手机号码登录，还可以使用支付宝登录，两者都能给予进入 app 所需的信息，满足登录要求。



#### 常规页面 

##### 消息

<img src="imgs/general-page/app-info.jpg" alt="消息页面" style="zoom:25%;" />

在一个应用中，界面的构成基本由多个部分组成。如上图所示，将消息界面分为由边框组成的几个主要部分，详情如下：

1. 应用级导航栏：该导航栏属于应用级导航，固定在应用底端，对应用提供的功能做最大类别的区分。在应用中，数据基本不会变化。
2. 消息视图：导航内容，该内容显示在界面中，但内容独立维护，可以在其他场景独立显示（以下简称视图）。
3. 视图操作区：该区域属于消息视图，用户定义消息视图的操作节点，不包括数据操作。
4. 视图搜索区：该区域属于消息视图，搜索消息数据。
5. 视图数据内容区：该区域属于消息视图，消息数据展示。

该界面结构的划分，是基于界面内容和界面功能的特性，将其模型化后，详情如下：

| 序号 | 名称           | 模型名称               | 详情                                                         | 备注             |
| ---- | -------------- | ---------------------- | ------------------------------------------------------------ | ---------------- |
| 1    | 应用级导航栏   | 应用菜单               | [ IPSAppMenu](https://modelapi.ibizlab.cn/#/net/ibizsys/model/control/menu/IPSAppMenu) |                  |
| 2    | 消息视图       | 应用视图               | [ IPSAppView](https://modelapi.ibizlab.cn/#/net/ibizsys/model/app/view/IPSAppView) |                  |
| 3    | 视图操作区     | 实体工具栏控件         | [ IPSDEToolbar](https://modelapi.ibizlab.cn/#/net/ibizsys/model/control/toolbar/IPSDEToolbar) |                  |
| 4    | 视图搜索区     | 快捷搜索               |                                                              | 应用视图内部模型 |
| 5    | 视图数据内容区 | 实体移动端多项数据控件 | [ IPSDEMobMDCtrl](https://modelapi.ibizlab.cn/#/net/ibizsys/model/control/list/IPSDEMobMDCtrl) |                  |

> 注：以下章节，不再介绍序号为 1 的应用级导航栏。



##### 日历

<img src="imgs/general-page/app-calendar.jpg" alt="日历" style="zoom:25%;" />









## 其他





