# IOS之分段控制器 -- OC/Swift4.0  

[![Platform](http://img.shields.io/badge/platform-iOS-blue.svg?style=flat)](http://cocoapods.org/?q=FWSegmentedControl)&nbsp;
![Language](https://img.shields.io/badge/language-swift-orange.svg?style=flat)&nbsp;
[![License](http://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://github.com/choiceyou/FWSegmentedControl/blob/master/FWSegmentedControl/LICENSE)



## 支持pod导入：

```swift
pod 'FWSegmentedControl'<br>
注意：如出现 Unable to find a specification for 'FWSegmentedControl' 错误，可执行 pod repo update 命令。
```



## 简单使用（注：可下载demo具体查看，分别有OC、Swift的demo）：  

```swift
/// 类初始化方法
///
/// - Parameters:
///   - scType: segment类型
///   - sectionTitleArray: 标题，可传nil，后续再设置
///   - sectionImageArray: 图片，可传nil，后续再设置
///   - sectionSelectedImageArray: 选中图片，可传nil，后续再设置
///   - frame: frame
@objc open class func segmentedWith(scType: SCType,
                                        scWidthStyle: SCWidthStyle,
                                        sectionTitleArray: [String]?,
                                        sectionImageArray: [UIImage]?,
                                        sectionSelectedImageArray: [UIImage]?,
                                        frame: CGRect) -> FWSegmentedControl
```

### OC：
```oc
[FWSegmentedControl segmentedWithScType:SCTypeText
                           scWidthStyle:SCWidthStyleDynamicFixedSuper
                      sectionTitleArray:@[@"关注", @"游戏", @"附近"]
                      sectionImageArray:nil sectionSelectedImageArray:nil
                                  frame:CGRectMake(0, 40, self.view.frame.size.width, 50)];
```


### Swift: <br>
```swift
FWSegmentedControl.segmentedWith(scType: SCType.text,
                           scWidthStyle: SCWidthStyle.fixed,
                      sectionTitleArray: ["关注", "游戏", "附近"],
                      sectionImageArray: nil,
              sectionSelectedImageArray: nil,
                                  frame: CGRect(x: 0, y: 40, width: Int(UIScreen.main.bounds.width), height: 50)) 

```



## 效果：

![](https://github.com/choiceyou/FWSegmentedControl/blob/master/%E7%A4%BA%E4%BE%8B1.gif)
![](https://github.com/choiceyou/FWSegmentedControl/blob/master/%E7%A4%BA%E4%BE%8B2.gif)



## 注意点：

一、本UI库是用Swift4.0编写的，所以安装或者拖入文件后需要把对应的Swift设置为4.0版本： <br>
（1）pod安装方式：![](https://github.com/choiceyou/FWSegmentedControl/blob/master/%E8%AE%BE%E7%BD%AE1.jpg)
（2）文件拖入方式：Targets --> Build Setting 做相同的设置

二、关于OC、Swift混编等相关问题，网上有很多相关解答，我这边就不再重复了



## 结尾语：

> * 使用过程中有任何问题或者新的需求都可以issues我哦；
> * 欢迎关注本人更多的UI库，谢谢；

