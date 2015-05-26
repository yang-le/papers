怎样移植CyanogenMod安卓系统到你的设备上
=======================================

关于移植的一些建议
------------------

嗯，你有一个手机或者平板或者其他什么东西，反正装的不是CyanogenMod安卓系统？

你以前在你的电脑上给其他的设备编译过CyanogenMod安卓系统，你觉得还挺好玩？甚至，你竟然还保留着源代码，准备弄出点更大的动静来？

好吧，你发光的机会到了！

> 注意
> ----

> _为方便起见，所有对目录的引用都假设你在源代码的根目录下（即你运行`repo init`的目录），目录名会相对于这里开始。如果你看了[编译说明](/Build_for_jordan.md)，源代码的根目录即是在`～/android/system`。_

先决条件
--------

移植CyanogenMod到新的设备上可能相当地简单，也可能相当地难。这将取决于设备本身，设备是否运行着一个较新的版本的安卓。当然，你作为一个开发者的技术，也很重要！

如果你之前没有为其他的设备编译过CyanogenMod（以及recovery），移植工作会非常难的。所以如果你真的还没编译过个一次两次的，现在就赶紧[试试](/Build_for_jordan.md)吧。

> 友情提示
> --------

> _如果你不是通过CyanogenMod Learning Center来到这个页面的,现在就可以去[Development](http://wiki.cyanogenmod.org/w/Development)获得更多信息。_

另外，你还应该确保自己熟悉CyanogenMod的源码结构。你应该知道，除了极少数的情况之外，几乎你所需要做的所有的事情都会发生在`/device/[vendor]/[codename]`，`/vendor/[vendor]/[codename]`以及`/kernel/[vendor]/[codename]`目录中。

> 友情提示
> --------

> _如欲了解关于CyanogenMod源码结构的更多信息，参考[这里](the_cm_source.md)。实际上，如果你计划做移植的话，最好是读读这篇文章。_

