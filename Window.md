# Window标签
## 属性
1. pos="xoffset,yoffset,width,height"  
> xoffset为控件水平锚点，yoffset为控件垂直锚点,width为宽度,height为高度(width,height取-1为参考子控件大小动态设置,-2为参考父控件,-0充满)  
>>- |*offset为参考居中父控件，取值范围为像素大小  
>>- %*offset为参考父窗口百分比位置,取值为0-100  
>>- [*offset / }*offset参考兄弟控件右边位置，取值为像素大小  
>>- ]*offset / {*offset参考兄弟控件左边位置，取值为像素大小  
>>- 注意事项当pos前两个取负数时为反向计算
2. skin="skin_name"
skin_name需要uires.idx先导入file再往skin.xml导入设定skin_name到图片映射，最后才可以使用例如  
> 使用前导入 uires.idx
>> \<IMG\>\<file name="img_login" path=""\>\</IMG\>  

> skin.xml
>> \<skin\><imglist name="skin_login" src="IMG:img_Login" /\>\</skin\>
3. cache="1" or cache="0"
>- 当cache=1会缓存窗口，用空间换时间
