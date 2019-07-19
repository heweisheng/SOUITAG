# Tabctrl标签
## 导航栏常用属性
1. tabHeight=""
>- 设置导航栏位置的大小
2. interpolator="Decelerate"
>- 可以加速动画，但是帧率会降低
3. curSel=""
>- 默认第几个窗口
4. foucable="0"
>- 点击标签时不会产生虚框
5. animateSteps=""
>- 设置动画帧数
6. animateType="1"
>- 背景跟着动 为0时不动（大概指的背景图）
7. text-y=""
>- 指定文字出现的位置，该属性一定要小于tabHeight，否则文字不会显示
8. icon-x=""
>- 指定导航栏的图标间隔
>>- 注意当聚焦框跟图标位置不在一起调整才有意义
9. colorTextHover="#ff0000" fontHover="italic:1"
>- 设置提示字体为xp版
## page子标签
1. title=""
>- 子标签的名字=按钮上的字
2. tip=""
>- 左键在控件附件会显示提升，为tip的内容
