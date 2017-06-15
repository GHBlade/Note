# CSS学习笔记
#### Tip
* `initial` 重置某个属性为UA(浏览器标识)默认设置
* `inherit` 继承父元素设置
* `-moz-` 代表Firefox(Gecko内核)浏览器私有属性      
  `-ms-`代表ie(ie内核)浏览器私有属性    
  `-webkit-`代表safari、chrome(webkit内核)私有属性   
  ```
  私有前缀是为了CSS新属性兼容各浏览器老版本的方式,通过这种方式来提前支持新属性,待w3c公布了标准后,再让新版浏览器支持不带私有前缀的写法。
  ```


#### 背景
 属性                    |  描述
------------------------ | -------------
background-attachment    |  背景图像是否固定或者随着页面的其余部分滚动(默认滚动)
background-color         |  设置元素的背景颜色
background-image         |  把图片设置为背景(默认重复排列)
background-position      |  设置背景图片的起始位置
background-repeat        |  设置背景图片是否及如何重复
background-size          |  规定背景图片的尺寸
background-origin        |  规定背景图片的定位区域
background-clip          |  规定背景图片的绘制区域

* background-repeat: space | round (可以定义两个值指定横向和竖向 space 固定 / round 调整)

#### 文本
属性                     |  描述
------------------------ | -------------
direcotion               |  文本方向
white-space              |  元素中空白的处理方式
text-align               |  文本对齐方式
word-spacing             |  字间距
letter-spacing           |  字符间距
text-decoration          |  对文本添加修饰
text-indent              |  缩进首行
text-transform           |  元素中的字母
unicode-bidi             |  设置文本方向
text-shadow              |  向文本添加阴影
word-wrap                |  规定文本的换行规则

* text-transform: capitalize(首字母大写) lowercase(小写) uppercase(大写)
* text-shadow: 左 上 清晰度 颜色
* word-wrap: normal  默认换行(断点字换行,没有断点会一直排下去)    break-word(在长单词或 URL 地址内部进行换行,不会截断单词,单词作为整体换行)
* word-break(规定非中日韩文本的换行规则): normal     
  break-all (截断换行)   keep-all(只能在半角空格或连字符处换行)

#### 字体
  属性                      |  描述
  ------------------------ | -------------
  font-style               |  字体风格
  font-variant             |  以小型大写字体或正常字体显示文本
  font-weight              |  设置字体的粗细

  ```CSS
    @font-face{
      font-family:myfont;
      src:url("...");
    }
  ```
  
#### 链接
  属性                      |  描述
  ------------------------ | -------------
  a:link                   |  普通的、未被访问的链接
  a:visited                |  用户已经访问的链接
  a:hover                  |  鼠标指正位于链接上方
  a:active                 |  链接被点击的时刻           

#### 列表
  属性                      |  描述
  ------------------------ | -------------
  list-style               |  简写列表项
  list-style-image         |  列表项图像
  list-style-position      |  列表标志位置
  list-style-type          |  列表类型  

#### 表格
  * tr 行   th 列头  td 列项
  * border-collapse:collapse  折叠边框

#### 轮廓
  属性                      |  描述
  ------------------------ | -------------
  outline                  |  设置轮廓属性
  outline-color            |  设置轮廓颜色
  outline-style            |  设置轮廓样式
  outline-width            |  设置轮廓宽度    
