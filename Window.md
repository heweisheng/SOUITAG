# Window标签
## 常用属性
1. pos="startx,starty,endx,endy"  
> x为控件水平锚点，y为控件垂直锚点 
>>- |为参考父控件居中位置，取值范围为像素大小  
>>- %为参考父窗口百分比位置,取值为0-100  
>>- [ / }参考兄弟控件右边位置，取值为像素大小  
>>- ] / {参考兄弟控件左边位置，取值为像素大小  
>>- 注意事项当pos取负数时为反向计算,后两个参数为空时按控件大小算
2. skin="skin_name"
skin_name需要uires.idx先导入file再往skin.xml导入设定skin_name到图片映射，最后才可以使用例如  
> 使用前导入 uires.idx
>> \<IMG\>\<file name="img_login" path=""\>\</IMG\>  

> skin.xml
>> \<skin\><imglist name="skin_login" src="IMG:img_Login" /\>\</skin\>
3. cache="1" or cache="0"
>- 当cache=1会缓存窗口，用空间换时间
4. layout="hbox" layout="vbox"
>- 水平布局，垂直布局，当设置了,子控件pos属性无效
5. colorBkgnd="#cccccc"
>- 背景色，与skin类似。
6. layout="gridLayout"
>- 网格布局，2.8特性，需要指定columnCount, rowCount, xInterval, yInterval, xGravity, yGravity等属性
>>- columnCount为指定行数
>>- rowCount为指定列数
>>- xInterval x轴间隔像素点
>>- yInterval y轴间隔像素点
