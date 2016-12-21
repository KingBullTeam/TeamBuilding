#  ES 6 学习入门指引

## ES6
* [箭头函数Arrow functions](http://babeljs.io/docs/learn-es2015/#arrows): `onPress={() => this.setState({pressed: true})}`
* 块级作用域Block scoping: `let greeting = 'hi';`

* 常量`Constants: const answer = 42;`
  * 声明的变量不允许重复声明，否则会报错 
  * let 和 const 不存在变量提升。
  * 要使对象为常量的话可以配合`Object.freeze()`函数来实现
  	 * 并不能冻结它的属性的属性被修改
  * **ES6规定，var命令和function命令声明的全局变量，属于全局对象的属性；let命令、const命令、class命令声明的全局变量，不属于全局对象的属性。**
  
* 数组的扩展运算Call spread: Math.max(...array);
  * 新增方法`Array.from()`
  * 新增方法`Array.of()`，用来将一组值转换为数组; `Array.of(3, 11, 8) // [3,11,8]`
  * 新增`find()`和`findIndex()`替代原来的`indexOf()`
  * 新增`fill()`,参数不同，含义不同
  * 新增数组实例方法：`ectries()`,`keys()`,`values()`,三个都返回遍历器

  
* 类Classes: class C extends React.Component { render() { return <View />; } }


* 动态属性键Computed Properties: var key = 'abc'; var obj = {[key]: 10};


* 解构Destructuring: const {isActive, style} = this.props;
	* 默认值  `const [num = 1024] = [undifined];`
	* 数组的解构
	* 对象结构
	
	```
	const { foo: baz } = { foo: "aaa", bar: "bbb" };
	baz // "aaa"
	```

* 对象方法的简写Object Consise Method: var obj = { method() { return 10; } };


* 对象属性的简写Object Short Notation: var name = 'vjeux'; var obj = { name };
  * Object.is()方法, 相对于运算符===有两个不同：一是+0不等于-0，二是NaN等于自身
  * bject.assign()方法

  
   
* 参数的扩展运算Rest Params: function(type, ...args) { }


* for...of: for (var num of [1, 2, 3]) {}


* 字符串模板Template Literals: var who = 'world'; var str = `Hello ${who}`;


* 模块Modules: import React, { Component } from 'react';
	* [export from MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/export)
	* [全面解析ECMAScript 6模块系统](http://www.csdn.net/article/2015-04-30/2824595-Modules-in-ES6)

* String.prototype.{startsWith, endsWith, repeat, includes}



## ES7
* 对象的扩展运算Object Spread: var extended = { ...obj, a: 10 };


* 参数列表末尾允许放置逗号Function Trailing Comma: function f(a, b, c,) { }


* Async函数: async function doStuffAsync() { const foo = await doOtherStuffAsync(); };


* Object.{entries, values}



## babel
* stage-0
* stage-1



参考资料

* [ES6 手册](https://qiutc.me/post/es6-cheatsheet.html#var_和_let/const_的比较)
* [JavaScript 编码规范-airbnb中文](http://www.kancloud.cn/kancloud/javascript-style-guide/43119)
* [airbnb/javascript](https://github.com/airbnb/javascript)
