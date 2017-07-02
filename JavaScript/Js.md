# JavaScript Array 对象
## Array
#### 对象属性
  属性	                    | 描 述
  ------------------------ | -------------
  constructor		           | 返回对创建此对象的数组函数的引用。
  length		               | 设置或返回数组中元素的数目。
  prototype		             | 使您有能力向对象添加属性和方法。

#### 对象方法
  方法		                  | 描 述
  ------------------------ | -------------
  concat()		             | 连接两个或更多的数组，并返回结果。
  join()		               | 把数组的所有元素放入一个字符串。元素通过指定的分隔符进行分隔。
  pop()		                 | 删除并返回数组的最后一个元素
  push()		               | 向数组的末尾添加一个或更多元素，并返回新的长度。
  reverse()		             | 颠倒数组中元素的顺序。
  shift()		               | 删除并返回数组的第一个元素
  slice()		               | 从某个已有的数组返回选定的元素
  sort()		               | 对数组的元素进行排序
  splice()		             | 删除元素，并向数组添加新元素。
  toSource()		           | 返回该对象的源代码。
  toString()		           | 把数组转换为字符串，并返回结果。
  toLocaleString()		     | 把数组转换为本地数组，并返回结果。
  unshift()		             | 向数组的开头添加一个或更多元素，并返回新的长度。
  valueOf()		             | 返回数组对象的原始值

## Boolean
#### 对象属性
  属性			                | 描述
  ------------------------ | -------------
  constructor			         | 返回对创建此对象的 Boolean 函数的引用
  prototype			           | 使您有能力向对象添加属性和方法。

#### 对象方法
  方法			                | 描述
  ------------------------ | -------------
  toSource()				       | 返回该对象的源代码。
  toString()				       | 把逻辑值转换为字符串，并返回结果。
  valueOf()				         | 返回 Boolean 对象的原始值。

## Date  
#### 对象属性
  属性			                | 描述
  ------------------------ | -------------
  constructor					     | 返回对创建此对象的 Date 函数的引用。
  prototype					       | 使您有能力向对象添加属性和方法。

#### 对象方法
  属性			                | 描述
  ------------------------ | -------------  
  Date()					         | 	返回当日的日期和时间。
  getDate()					       | 	从 Date 对象返回一个月中的某一天 (1 ~ 31)。
  getDay()					       | 	从 Date 对象返回一周中的某一天 (0 ~ 6)。
  getMonth()					     | 	从 Date 对象返回月份 (0 ~ 11)。
  getFullYear()					   | 	从 Date 对象以四位数字返回年份。
  getYear()					       | 	请使用 getFullYear()方法代替。
  getHours()					     | 	返回 Date 对象的小时 (0 ~ 23)。
  getMinutes()					   | 	返回 Date 对象的分钟 (0 ~ 59)。
  getSeconds()					   | 	返回 Date 对象的秒数 (0 ~ 59)。
  getMilliseconds()				 | 	返回 Date 对象的毫秒(0 ~ 999)。
  getTime()					       | 	返回 1970 年 1 月 1 日至今的毫秒数。
  getTimezoneOffset()		   | 	返回本地时间与格林威治标准时间 (GMT) 的分钟差。
  getUTCDate()					   | 	根据世界时从 Date 对象返回月中的一天 (1 ~ 31)。
  getUTCDay()					     | 	根据世界时从 Date 对象返回周中的一天 (0 ~ 6)。
  getUTCMonth()					   | 	根据世界时从 Date 对象返回月份 (0 ~ 11)。
  getUTCFullYear()				 | 	根据世界时从 Date 对象返回四位数的年份。
  getUTCHours()					   | 	根据世界时返回 Date 对象的小时 (0 ~ 23)。
  getUTCMinutes()					 | 	根据世界时返回 Date 对象的分钟 (0 ~ 59)。
  getUTCSeconds()					 | 	根据世界时返回 Date 对象的秒钟 (0 ~ 59)。
  getUTCMilliseconds()		 | 	根据世界时返回 Date 对象的毫秒(0 ~ 999)。
  parse()					         | 	返回1970年1月1日午夜到指定日期（字符串）的毫秒数。
  setDate()					       | 	设置 Date 对象中月的某一天 (1 ~ 31)。
  setMonth()					     | 	设置 Date 对象中月份 (0 ~ 11)。
  setFullYear()					   | 	设置 Date 对象中的年份（四位数字）。
  setYear()					       | 	请使用 setFullYear()	方法代替。
  setHours()					     | 	设置 Date 对象中的小时 (0 ~ 23)。
  setMinutes()					   | 	设置 Date 对象中的分钟 (0 ~ 59)。
  setSeconds()					   | 	设置 Date 对象中的秒钟 (0 ~ 59)。
  setMilliseconds()				 | 	设置 Date 对象中的毫秒 (0 ~ 999)。
  setTime()					       | 	以毫秒设置 Date 对象。
  setUTCDate()					   | 	根据世界时设置 Date 对象中月份的一天 (1 ~ 31)。
  setUTCMonth()					   | 	根据世界时设置 Date 对象中的月份 (0 ~ 11)。
  setUTCFullYear()			   | 	根据世界时设置 Date 对象中的年份（四位数字）。
  setUTCHours()					   | 	根据世界时设置 Date 对象中的小时 (0 ~ 23)。
  setUTCMinutes()					 | 	根据世界时设置 Date 对象中的分钟 (0 ~ 59)。
  setUTCSeconds()					 | 	根据世界时设置 Date 对象中的秒钟 (0 ~ 59)。
  setUTCMilliseconds()	   | 	根据世界时设置 Date 对象中的毫秒 (0 ~ 999)。
  toSource()					     | 	返回该对象的源代码。
  toString()					     | 	把 Date 对象转换为字符串。
  toTimeString()					 | 	把 Date 对象的时间部分转换为字符串。
  toDateString()					 | 	把 Date 对象的日期部分转换为字符串。
  toGMTString()					   | 	请使用 toUTCString()方法代替。
  toUTCString()					   | 	根据世界时，把 Date 对象转换为字符串。
  toLocaleString()				 | 	根据本地时间格式，把 Date 对象转换为字符串。
  toLocaleTimeString()		 | 	根据本地时间格式，把 Date 对象的时间部分转换为字符串。
  toLocaleDateString()		 | 	根据本地时间格式，把 Date 对象的日期部分转换为字符串。
  UTC()					           | 	根据世界时返回 1970 年 1 月 1 日 到指定日期的毫秒数。
  valueOf()					       | 	返回 Date 对象的原始值。

## Math   
#### 对象属性
  属性			                | 描述  
  ------------------------ | -------------
  E						             | 	返回算术常量 e，即自然对数的底数（约等于2.718）。
  LN2						           | 	返回 2 的自然对数（约等于0.693）。
  LN10						         | 	返回 10 的自然对数（约等于2.302）。
  LOG2E						         | 	返回以 2 为底的 e 的对数（约等于 1.414）。
  LOG10E						       | 	返回以 10 为底的 e 的对数（约等于0.434）。
  PI						           | 	返回圆周率（约等于3.14159）。
  SQRT1_2						       | 	返回返回 2 的平方根的倒数（约等于 0.707）。
  SQRT2						         | 	返回 2 的平方根（约等于 1.414）。
#### 对象方法
  属性			                | 描述  
  ------------------------ | -------------
  abs(x)				           | 返回数的绝对值。
  acos(x)				           | 返回数的反余弦值。
  asin(x)				           | 返回数的反正弦值。
  atan(x)				           | 以介于 -PI/2 与 PI/2 弧度之间的数值来返回 x 的反正切值。
  atan2(y,x)				       | 返回从 x 轴到点 (x,y) 的角度（介于 -PI/2 与 PI/2 弧度之间）。
  ceil(x)				           | 对数进行上舍入。
  cos(x)				           | 返回数的余弦。
  exp(x)				           | 返回 e 的指数。
  floor(x)				         | 对数进行下舍入。
  log(x)				           | 返回数的自然对数（底为e）。
  max(x,y)				         | 返回 x 和 y 中的最高值。
  min(x,y)				         | 返回 x 和 y 中的最低值。
  pow(x,y)				         | 返回 x 的 y 次幂。
  random()				         | 返回 0 ~ 1 之间的随机数。
  round(x)				         | 把数四舍五入为最接近的整数。
  sin(x)				           | 返回数的正弦。
  sqrt(x)				           | 返回数的平方根。
  tan(x)				           | 返回角的正切。
  toSource()				       | 返回该对象的源代码。
  valueOf()				         | 返回 Math 对象的原始值。

## Number    
#### 对象属性
  属性			                | 描述  
  ------------------------ | -------------
  constructor					     | 返回对创建此对象的 Number 函数的引用。
  MAX_VALUE					       | 可表示的最大的数。
  MIN_VALUE					       | 可表示的最小的数。
  NaN					             | 非数字值。
  NEGATIVE_INFINITY				 | 负无穷大，溢出时返回该值。
  POSITIVE_INFINITY				 | 正无穷大，溢出时返回该值。
  prototype					       | 使您有能力向对象添加属性和方法。

#### 对象方法
  属性			                | 描述  
  ------------------------ | -------------
  toString				         | 把数字转换为字符串，使用指定的基数。
  toLocaleString				   | 把数字转换为字符串，使用本地数字格式顺序。
  toFixed				           | 把数字转换为字符串，结果的小数点后有指定位数的数字。
  toExponential				     | 把对象的值转换为指数计数法。
  toPrecision				       | 把数字格式化为指定的长度。
  valueOf				           | 返回一个 Number 对象的基本数字值。

## String     
#### 对象属性
  属性			                | 描述  
  ------------------------ | -------------
  constructor				       | 对创建该对象的函数的引用
  length				           | 字符串的长度
  prototype				         | 允许您向对象添加属性和方法

#### 对象方法
  属性			                | 描述  
  ------------------------ | -------------  
  anchor()				         |	创建 HTML 锚。
  big()				             |	用大号字体显示字符串。
  blink()				           |	显示闪动字符串。
  bold()				           |	使用粗体显示字符串。
  charAt()				         |	返回在指定位置的字符。
  charCodeAt()				     |	返回在指定的位置的字符的 Unicode 编码。
  concat()				         |	连接字符串。
  fixed()				           |	以打字机文本显示字符串。
  fontcolor()				       |	使用指定的颜色来显示字符串。
  fontsize()				       |	使用指定的尺寸来显示字符串。
  fromCharCode()				   |	从字符编码创建一个字符串。
  indexOf()				         |	检索字符串。
  italics()				         |	使用斜体显示字符串。
  lastIndexOf()				     |	从后向前搜索字符串。
  link()				           |	将字符串显示为链接。
  localeCompare()				   |	用本地特定的顺序来比较两个字符串。
  match()				           |	找到一个或多个正则表达式的匹配。
  replace()				         |	替换与正则表达式匹配的子串。
  search()				         |	检索与正则表达式相匹配的值。
  slice()				           |	提取字符串的片断，并在新的字符串中返回被提取的部分。
  small()				           |	使用小字号来显示字符串。
  split()				           |	把字符串分割为字符串数组。
  strike()				         |	使用删除线来显示字符串。
  sub()				             |	把字符串显示为下标。
  substr()				         |	从起始索引号提取字符串中指定数目的字符。
  substring()				       |	提取字符串中两个指定的索引号之间的字符。
  sup()				             |	把字符串显示为上标。
  toLocaleLowerCase()			 |	把字符串转换为小写。
  toLocaleUpperCase()			 |	把字符串转换为大写。
  toLowerCase()				     |	把字符串转换为小写。
  toUpperCase()				     |	把字符串转换为大写。
  toSource()				       |	代表对象的源代码。
  toString()				       |	返回字符串。
  valueOf()				         |	返回某个字符串对象的原始值。

## RegExp      
#### 修饰符
  修饰符			         | 描述  
  -----------------  | -------------
  i					         |	执行对大小写不敏感的匹配。
  g					         |	执行全局匹配（查找所有匹配而非在找到第一个匹配后停止）。
  m					         |	执行多行匹配。

#### 方括号
  表达式				             | 描述
  ------------------------ | -------------  
  [abc]				             | 查找方括号之间的任何字符。
  [^abc]				           | 查找任何不在方括号之间的字符。
  [0-9]				             | 查找任何从 0 至 9 的数字。
  [a-z]				             | 查找任何从小写 a 到小写 z 的字符。
  [A-Z]				             | 查找任何从大写 A 到大写 Z 的字符。
  [A-z]				             | 查找任何从大写 A 到小写 z 的字符。
  [adgk]				           | 查找给定集合内的任何字符。
  [^adgk]				           | 查找给定集合外的任何字符。
  (red|blue|green)				 | 查找任何指定的选项。

#### 元字符
  元字符			         | 描述  
  ------------------------ | -------------
  .				                 | 查找单个字符，除了换行和行结束符。
  \w					             | 查找单词字符。
  \W					             | 查找非单词字符。
  \d					             | 查找数字。
  \D					             | 查找非数字字符。
  \s					             | 查找空白字符。
  \S					             | 查找非空白字符。
  \b					             | 匹配单词边界。
  \B					             | 匹配非单词边界。
  \0					             | 查找 NUL 字符。
  \n					             | 查找换行符。
  \f					             | 查找换页符。
  \r					             | 查找回车符。
  \t					             | 查找制表符。
  \v					             | 查找垂直制表符。
  \xxx					           | 查找以八进制数 xxx 规定的字符。
  \xdd					           | 查找以十六进制数 dd 规定的字符。
  \uxxxx					         | 查找以十六进制数 xxxx 规定的 Unicode 字符。


#### 量词
  量词			            | 描述  
  -------------------  | -------------
  n+					         | 匹配任何包含至少一个 n 的字符串。
  n*					         | 匹配任何包含零个或多个 n 的字符串。
  n?					         | 匹配任何包含零个或一个 n 的字符串。
  n{X}					       | 匹配包含 X 个 n 的序列的字符串。
  n{X,Y}					     | 匹配包含 X 至 Y 个 n 的序列的字符串。
  n{X,}					       | 匹配包含至少 X 个 n 的序列的字符串。
  n$					         | 匹配任何结尾为 n 的字符串。
  ^n					         | 匹配任何开头为 n 的字符串。
  ?=n					         | 匹配任何其后紧接指定字符串 n 的字符串。
  ?!n					         | 匹配任何其后没有紧接指定字符串 n 的字符串。

#### RegExp 对象属性
  属性			         | 描述  
  -----------------  | -------------
  global					   | RegExp 对象是否具有标志 g。	 
  ignoreCase				 | RegExp 对象是否具有标志 i。	 
  lastIndex					 | 一个整数，标示开始下一次匹配的字符位置。	 
  multiline					 | RegExp 对象是否具有标志 m。
  source					   | 正则表达式的源文本。

#### RegExp 对象方法
  方法			         | 描述  
  -----------------  | -------------
  compile					   | 编译正则表达式。
  exec						   | 检索字符串中指定的值。返回找到的值，并确定其位置。
  test						   | 检索字符串中指定的值。返回 true 或 false。

#### 支持正则表达式的 String 对象的方法
  方法			         | 描述
  ----------------- | -------------
  search						| 检索与正则表达式相匹配的值。	 
  match							| 找到一个或多个正则表达式的匹配。	 
  replace						| 替换与正则表达式匹配的子串。	 
  split							| 把字符串分割为字符串数组。

## Functions
####   顶层函数（全局函数）
  函数				           |描述
  --------------------- | -------------
  decodeURI()						| 解码某个编码的 URI。
  decodeURIComponent()	| 解码一个编码的 URI 组件。
  encodeURI()						| 把字符串编码为 URI。
  encodeURIComponent()	| 把字符串编码为 URI 组件。
  escape()							| 对字符串进行编码。
  eval()							  | 计算 JavaScript 字符串，并把它作为脚本代码来执行。
  getClass()						| 返回一个 JavaObject 的 JavaClass。
  isFinite()						| 检查某个值是否为有穷大的数。
  isNaN()							  | 检查某个值是否是数字。
  Number()							| 把对象的值转换为数字。
  parseFloat()					| 解析一个字符串并返回一个浮点数。
  parseInt()						| 解析一个字符串并返回一个整数。
  String()							| 把对象的值转换为字符串。
  unescape()						| 对由 escape() 编码的字符串进行解码。
####   顶层属性（全局属性）
  函数				           |描述
  --------------------- | -------------
  Infinity							| 代表正的无穷大的数值。
  java								  | 代表 java.* 包层级的一个 JavaPackage。
  NaN								    | 指示某个值是不是数字值。
  Packages						  | 根 JavaPackage 对象。
  undefined						  | 指示未定义的值。
