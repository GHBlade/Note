# Flex布局
* 容器：flex-container  项目：flex-item  主轴：main axis  十字轴(纵轴)：cross axis
  起点：start  终点：end

* display : flex  (flex布局并同一行显示)  / inline-flex (宽度为内容宽度)
* flex-direction 设置主轴方向  row 水平方向(row-reverse 水平反向)   / column  垂直方向（column-reverse 垂直反向）
* flex-wrap ：wrap 控制是否多行显示（自动换行） / wrap-reverse (颠倒每排内容位置)
* flex-flow: (flex-direction) (flex-wrap) ; (默认：row no-wrap)
* justify-content:调整项目位置，项目跟项目间的间隔
  justify-content: flex-start/ flex-end / center / space-between(等分，左右无间隔) / space-around(等分，左右有间隔)
* align-items: 项目垂直方向的对齐方式
  align-items: stretch (默认：拉伸)/ flex-start(垂直轴起点)/ flex-end /center / baseline(内容基线对齐)
* align-content:项目多行显示，调整垂直方向对齐方式
  align-content:stretch (默认：拉伸)/flex-start(垂直轴起点)/ flex-end /center / space-between/space-around
* order : 项目排序  order: .../ -1 / 0 (默认)/ 1 / 2 / ...
* flex-grow : 0 (默认)  按比例划分剩余空间
* flex-basis : auto (默认) 项目初始宽度  
* flex-shrink : 0 ; 收缩宽度不收影响     3: 按3倍比例收缩
* flex: (flex-grow) (flex-shrink) （flex-basis)
* align-self:单独控制某一个项目的位置 在单独项目(元素)中使用
  align-self:auto (默认)/stretch / flex-start(垂直轴起点)/ flex-end /center
