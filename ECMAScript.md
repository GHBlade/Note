# ES6(ES2015)
*  块级作用域`let` :作用域外不能调用
*  恒量`const`:非自定义对象初始化后不能更改其值,自定义对象可以更改对象属性
*  解构数组：
```javaScript
  let [a,b,c] = ['1','2','3'];
```
*  解构对象：
```javaScript
  let {a,b,c} = {a='1',b='2',c='3'};
```
* 模板字符串：
```javaScript
  let a = 'nick',
      b = 20;
  // 可以转行显示
  let info = `姓名${a}年龄${b}`;
```
* 带标签的模板字符串:
```javaScript
  // 上方代码
  ...
  let info = test`姓名${a}年龄${b}!`;
  function test(strings,...values){
    // console.log(strings);
    // console.log(values);
    let result = '';
    for(var i=0;i<values.length;i++){
      result += strings[i];
      result += values[i];
    }
    result += strings[strings.length-1];
    return result;
  }
```
* 判断字符串里是否包含其他字符串:
```javaScript
  // 上方代码
  ...
  console.log(info.startsWith('姓名'));// true
  console.log(info.endsWith('!'));// true
  console.log(info.includes('nick'));// true
```
* 默认参数:
```javaScript
  // 上方代码
  ...
  function show(a = 'jack' , b = 18){
    return `${a},${b}`;
  }
```
* 展开操作符Spread(...):
```javaScript
  // 上方代码
  ...
  let info = ['nick','jack'],
      list = ['cat',...info];

  console.log(...info);
  console.log(...list);
```
* 剩余操作符Rest(...):
```javaScript
  // 上方代码
  ...  
  // 这里参数的...表示Rest操作符
  function show(a,b,...c){
    console.log(a,b,c);
    console.log(a,b,...c);//这里的...表示Spread操作符
  }
  show(1,2,3,4,5,6,7);
```
* 解构参数:
```javaScript
  // 上方代码
  ...  
  // 最后的参数给定空白对象 这样可以不传{c,d}的值
  function show(a,b,{c,d} = {}){
    console.log(a,b,c,d);
  }
  show(1,2,{c=3,d=4});
```
* 函数的名字-name属性:
```javaScript
  // 上方代码
  ...  
  let test = function(args){
    ...
  }
  let show = function superShow(args){
    ...
  }

  console.log(test.name);//test
  console.log(show.name);//superShow
```
* 箭头函数 ArrowFunctions:
```javaScript
  // 上方代码
  ...  
  let  show = () => getSomething;
  let  show = (a,b) => getSomething + a + b ;
  let  show = (a,b) => {
    return a + b;
  } ;
```
* 对象表达式:
```javaScript
  // 上方代码
  ...  
  let  a = 1, b=2;
  let  c = {
            a,
            b,
            show(){}
          };
  console.log(c); // c.a  c.b   c.show()       
```
* 对象属性名:
```javaScript
  // 上方代码
  ...  
  let a = {};
  let b = 'get age';
  a.name = 'nick';
  // 带空格的属性名
  a['get age'] = 20;
  a[b] = 20;
  console.log(a);
```
* 对比两个值是否相等:
```javaScript
  // 上方代码
  ...  
  +0 == -0; // true
  +0 === -0;// true
  NaN == NaN; // false
  Object.is(NaN,NaN);// true
  Object.is(+0,-0);//false
```
* 把对象的值复制到另一个对象里Object.assign():
```javaScript
  // 上方代码
  ...  
  let a = {};
  Object.assign(
    a,{b:'20'}
  );
  console.log(a);
```
* 设置对象的prototype:
```javaScript
  // 上方代码
  ...  
  let a = {
    show(){
      return 10;
    }
  };
  let b = {
    show(){
      return 20;
    }
  };

  let c = Object.create(a);
  console.log(c.show()); //10
  console.log(c.getPrototypeOf(c) === a); // true

  Object.setPrototypeOf(c,b);
  console.log(c.show());// 20
```
* `__proto__`:
```javaScript
  // 上方代码
  ...  
  let c = {
    __proto__ : a
  };

  console.log(c.show);
  console.log(c.getPrototypeOf(c) === a); // true
  c.__proto__ = b;
  console.log(c.show());// 20
```
* super:
```javaScript
  // 上方代码
  ...  
  let c = {
    __proto__ : a,
    show(){
      return super.show() + 20;
    }
  }
  console.log(c.show());// 10+20 =30
```
* 迭代器Iterators:
```javaScript
  // 上方代码
  ...  
  function show(peoples){
    let i = 0;
    return {
      next(){
        let done = (i >= peopels.length);
        let value = !done ? peoples[i++] : undefined;

        return {
          value: value,
          done: done
        }
      }
    }
  }

  let list = show(['nick','jack','andy']);
  console.log(list.next());
  console.log(list.next());
```
* 生成器Generators:
```javaScript
  // 上方代码
  ...  
  // *  yield
  function* show(peoples){
    for(var i = 0; i< peoples.length ; i++){
      yield peoples[i];
    }
  }

  let list = show(['nick','jack']);
  console.log(list.next());
```
* 类Classes:
```javaScript
   class Student{
     constructor(name){
       this.name = name;
     }
     show(){
       console.log(this.name);
     }
   }

   let a = new Student('nick');
   a.show();
```
* get与set:
```javaScript
   class Student{
     constructor(name){
       this.name = name;
       this.friends = [];
     }
     show(){
       console.log(this.name);
     }
     get friend(){
       return this.friends;
     }

     set friend(friends){
       this.friends.push(friends);
     }
   }

   let a = new Student('nick');
   console.log(a.friend = 'jack');
   console.log(a.friend = 'andy');
   console.log(a.friend);
```
* 静态方法static:
```javaScript
   class Student{
     constructor(name){
       this.name = name;
       this.friends = [];
     }
     static show(age){
       console.log(age);
     }
     get friend(){
       return this.friends;
     }

     set friend(friends){
       this.friends.push(friends);
     }
   }

   Student.show(10);
```
* 继承extends:
```javaScript
   class Person{
     constructor(name,age){
       this.name = name;
       this.age = age;
     }
     show(){
       return `${this.name},${this.age}`;
     }
   }

   class Student extends Person{
     constructor(name,age){
       super(name,age);
     }
   }

   let a = new Student('nick',20);
   console.log(a.show());
```
* Set:
```javaScript
   // set 不能包含重复值
   let a = new Set('nick','jack');
   a.add('andy');
   console.log(a);
   console.log(a.size);
   console.log(a.has('andy'));
   a.delete('andy');
   console.log(a);
   a.forEach(item=>{
     console.log(item);
   });
   a.clear();
```
* Map:
```javaScript
   let a = new Map();
   let b = {},c = function(){},d = 'hello';
   a.set(b,'name');
   a.set(c,'age');
   a.set(d,'intro');

   console.log(a);
   console.log(a.size);
   console.log(a.get(b));
   console.log(a.get(c));
   a.delete(d);
   a.forEach((value,key) =>{
     console.log(`${key} = ${value}`);
   });
   a.clear();
```
* Module:
```javaScript
   // module A
   let a = "nick",
   let b = 20;

   export {a,b};
   // module B
   import {a,b} from './A';
  //  import * as A from './A';
   console.log(a,b);
  //  console.log(A.a,A.b);
```
* 重命名导出与导入的东西:
```javaScript
   // module A
   let a = "nick",
   let b = 20;
   function show(a,b){
     console.log(`姓名：${a},年龄：${b}`);
   }
   export {a,b,show as supper};
   // module B
   import {a,b,supper as open} from './A';
   open(a,b);
```
* 默认导出与导入:
```javaScript
   // module A
   let a = "nick",
   let b = 20;
   export default function show(a,b){
     console.log(`姓名：${a},年龄：${b}`);
   }

  // export default show;
  // export {show as default}; 

   // module B
   import show from './A';
  //  import open from './A';
   show('nick',20);
```
