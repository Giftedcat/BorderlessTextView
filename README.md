代码来源：https://github.com/domain9065/MultiplTextView
修改最低支持版本，自用

- # 简介
>BorderlessTextView  是一个通过重写TextView实现去除原生默认内边距，并扩展了一些其他功能的Android TextView。

## BorderlessTextView 扩展功能
- 去除原生textview默认边距
- 字体颜色渐变
- 字体闪动颜色
- 设置字体样式
## BorderlessTextView 实现效果
![效果图](/doc/introduction.gif)

# 使用

## 添加依赖
1. 在project的build.gradle 添加远程仓库源 jitpack.io
```
allprojects {
    repositories {
        google()
        jcenter()
        //配置 JitPack 插件的仓库地址
        maven { url "https://jitpack.io" }
    }
}
```
2. 在moudle app 的build.gradle 添加本库依赖 
- gradle3.0之后
```
implementation 'com.github.Giftedcat:BorderlessTextview:v1.0.0'
```

- gradle3.0之前

```
compile 'com.github.Giftedcat:BorderlessTextview:v1.0.0'
```

## xml可使用属性

属性 | 值 | 描述
---|---|---
app:runText | ture/false | 设置文字是否闪动
app:gradient | ture/false | 设置文字是否渐变
app:removeDefaultPadding | ture/false | 设置文字是否移除默认边距
app:gradientStartColor | #FFFF00 | 设置渐变或者闪动时开头颜色
app:gradientCenterColor | #FFFF00 | 设置渐变或者闪动时中间颜色
app:gradientEndColor | #FFFF00 | 设置渐变或者闪动时结束颜色
app:textFont | font/source.OTF | 设置textview的字体,source.otf字体需要放在project视图下的main下面的assets的font文件夹，没有就新建一个。值为这个字体的路径。



