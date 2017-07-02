# Js学习笔记
#### 数组操作
* push() 添加到最后  
* pop() 删除最后一个并返回该值
* shift() 删除第一个并返回该值
* delete arr[x] 删除掉序号为x的数值，数组长度不变
* splice(x) 删除掉序号为x的数据，长度-1
* arr1.concat(arr2) 合并两个数组

#### 遍历
* for in  (Array)  
  ```
    存在问题:
    1.index索引为字符串型数字，不能直接进行几何运算
    2.遍历顺序有可能不是按照实际数组的内部顺序
    3.使用for in会遍历数组所有的可枚举属性，包括原型。例如method和name属性
     所以for in更适合遍历对象，不要使用for in遍历数组
  ```
* for of (Array)
 ```
  记住，for in遍历的是数组的索引（即键名），而for of遍历的是数组元素值   
  for of遍历的只是数组内的元素，而不包括数组的原型属性method和索引name
  遍历对象 通常用for in来遍历对象的键名

  for in 可以遍历到Object的原型方法method,如果不想遍历原型方法和属性的话，可以在循环内部判断一下,hasOwnPropery方法可以判断某属性是否是该对象的实例属性

  可以通过ES5的Object.keys(myObject)获取对象的实例属性组成的数组，不包括原型方法和属性
 ```

#### 对象
* property (属性)
* method (方法)
```
  detele 对象.属性 会删除掉该对象的属性
```

#### DOM操作
 * querySelector  (返回单个查询结果)
 * querySelectorAll (返回所有查询结果)
 * element.previousElementSibling (元素节点上一个兄弟节点)
 * element.nextElementSibling (元素节点下一个兄弟节点)
 * element.childNodes  (获取子节点数组)
 * element.innerText  (文本内容 不含节点标签)
 * element.childElementCount （子节点个数)
 * element.firstElementChild  (返回第一个)  listElementChild (返回最后一个)
 * document.creatElement('...') (创建节点)
 * document.creatTextNode('...') (创建文本节点)
 * elment.appendChild(node) (插入节点到最后)
 * elment.removeChild(node) (删除指定子节点node)
 * elment.insertBefore(node,elment.firstChild) (在指定位置插入节点)

#### Event 事件(常用)
 * 冒泡型事件的基本思想是、事件按照从最特定的事件目标到最不特定的事件目标(document对象)的顺序触发
 * 捕获型事件中,事件从最不精确的对象(document对象)开始触发、然后到最精确
 * 事件触发顺序  捕获型事件->冒泡型事件(两种事件流都会触发DOM中的所有对象，从document对象开始，也在document对象结束)
 ```
 DOM事件模型的最独特的性质是，文本节点也触发事件(在IE不会)
 ```
 * addEventListener(event, function, useCapture) (为对象绑定事件监听)
 ```
    指定事件是否在捕获或冒泡阶段执，true 捕获阶段执行  false(默认) 冒泡阶段执行
 ```
 * removeEventListener() (移除 addEventListener() 方法添加的事件句柄)
 * event.stopPropagation() (阻止事件的继续传播 (中断传播))
