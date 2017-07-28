# CocosCreator-Toast
本人刚开始使用JavaScript和CocosCreator不久,希望大家提出bug和意见。

## 效果演示
类似于Android的Toast控件,显示在当前运行的Scene的Canvas上。
![](/doc/2.gif)

可以设置显示的文本、时长、位置、背景图片.
## 使用方法

### 1.导入项目
把Toast.js文件导入到你的Cococs Creator项目中，选中此文件，并在最右侧的“属性检查器”中勾选“导入为插件”。如下图：

![](/doc/1.png)

这样就可以全局使用Toast控件了，当然你也可以不勾选“导入为插件”，不过这样你必须在使用Toast之前对文件进行引用。


### 2.使用代码
#### a方式：
    //  设置显示文本与显示时间
    var toast = Toast.makeText('Toast', Toast.LENGTH_SHORT);
    //  设置位置与x,y的偏移方向
    toast.setGravity(Toast.CENTER, 0, 0);
    //  显示
    toast.show();
### b方式：
    //  设置文本与时间,直接显示
    Toast.showText('Toast', Toast.LENGTH_LONG);
    //  或
    Toast.makeText('Toast', Toast.LENGTH_SHORT).show();

    

