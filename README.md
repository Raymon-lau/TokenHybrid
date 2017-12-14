# TokenHybrid


![](http://ou3yprhbt.bkt.clouddn.com/hybridBanner.png)
![](https://img.shields.io/badge/language-ObjectiveC-orange.svg) ![](https://img.shields.io/badge/platform-iOS9+-blue.svg) ![](https://img.shields.io/dub/l/vibe-d.svg) ![](https://img.shields.io/cocoapods/v/TokenHybrid.svg?style=flat)

------------------------
## TokenHybrid是什么

**TokenHybrid** 是一个可以让你**脱离服务器**，使用HTML,CSS,JS构建iOS 原生界面的库，**帮你解除以下烦恼**

1. 不在为了修复一个小BUG 或者为更新一点内容就得去app store 审核，跳过这个漫长的过程。
2. 不再依赖服务器，自己控制app 的内容，动态更新界面或者功能，给用户创造彩蛋，吸引用户。
3. H5应用存在首屏加载时间慢，即使做的再好，也很难有原生的体验。

工作原理：**TokenHybrid** 解析一个HTML 文本，并根据这个HTML 下载相应的CSS，JS 并且构建原生界面，使用JS交互。

如何不使用服务器？
将你编写好的HTML，CSS,JS文件放在github，获取row地址传给TokenHybrid就可以！
之后更新App，只需修改HTML，CSS,JS并且push 到github即可。

`TokenHybrid` 里面的代码你可以随意修改。作者水平有限，希望能和大家共同进步。希望收到你对这个想法的意见，代码改进建议或者PR


## TokenHybrid 特性

1. 独立开发者的更新程序不再依赖服务器！
2. 首屏加载速度快，远超webView，并且自动缓存，甚至包括视图结构的坐标信息，不需要第二次计算！
2. 轻量级，可扩展性高，既可以嵌入页面，也可以完全用来开发页面程序！
3. 支持大部分HTML 标准，支持CSS，布局使用CSS的Flex！
4. 当HTML 更新的时候，重新打开界面会自动生成新界面！

## 预览
以下所有界面，都使用TokenHybrid 构建，最后有GIF图
图片中所有HTML源码在    [这里](https://github.com/cx478815108/TokenHybridHTML)
![](http://ou3yprhbt.bkt.clouddn.com/tokenhybrid.png)
![](https://raw.githubusercontent.com/cx478815108/TokenHybrid/master/screenshots/example.gif)


------------------------
## How to use

```
- (IBAction)start:(id)sender {
    NSString *url = @"your html url";   
    TokenHybridRenderController *obj = [[TokenHybridRenderController alloc] initWithHTMLURL:url];
    [self.navigationController pushViewController:obj animated:YES];
}
```

## Install & Run

Clone this project and run in Xcode9

Install

```
pod 'TokenHybrid'
```

## API使用
请看Document文件夹

### 手动安装

[下载这个Demo](https://github.com/cx478815108/TokenHybrid/archive/master.zip) 将 工程里面的 `TokenExtension`和`source` 文件夹拖入你的项目即可，依赖的库你可以根据你自己的需要选择去掉或者保留。

## 联系我

[XiongChen](mailto:feelings0811@wutnews.net) -> feelings0811@wutnews.net


