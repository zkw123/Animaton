# Anime
主要针对原本动画中存在的bug进行了修改，并增加了两种跳跃模式：按住空格会进行大跳，滞空时间长，跳跃较高，且有滞空的动画，点击空格进行普通跳跃，滞空时间短，跳跃较低，没有滞空动画。解决了原来的跳跃仅播放动画人物不移动的bug，以及下蹲人物会自动行走的bug，操作方式保持不变。基本实现了人物的基础动作表现。
因为传统fps游戏中跳跃的同时可以进行位移，所以跳跃使用了脚本驱动而非动画驱动（不然就只能在y轴移动），另外将Crouch Tree中的idle crouching坐标值修改为0来解决下蹲移动的bug。
代码位于/animation/Assets/NaughtyCharacter/Scripts目录下，主要对Character.cs进行了修改。生成的可执行文件位于animation/Game目录下
