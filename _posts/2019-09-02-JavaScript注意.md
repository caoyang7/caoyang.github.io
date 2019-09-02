---
layout: post
title: "JavaScript注意事项"
date: 2019-9-02 13:26:40
image: 'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=1259821177,3195294575&fm=26&gp=0.jpg'
description: JavaScript注意事项
category: 'blog'
tags:
- JavaScript
introduction: JavaScript注意事项
---

1. 改变颜色  
    x=document.getElementById("demo");  
    x.style.color="#ff0000";  

2. 验证输入是不是数字  
    if isNaN(x) {alert("不是数字")};  

3. 	那些老旧的实例可能会在 <script> 标签中使用 type="text/javascript"。现在已经不必这样做了。JavaScript 是所有现代浏览器以及 HTML5 中的默认脚本语言。  

4. JavaScript输出  
    使用 window.alert() 弹出警告框。  
    使用 document.write() 方法将内容写到 HTML 文档中。  
    使用 innerHTML 写入到 HTML 元素。  
    使用 console.log() 写入到浏览器的控制台。  

5. 请使用 document.write() 仅仅向文档输出写内容。  
    如果在文档已完成加载后执行 document.write，整个 HTML 页面将被覆盖。  

6. console.log() 方法能够让你看到你在页面中的输出内容，让你更容易调试javascript；与alert相比，console不会打断你页面的操作，console里面的内容非常丰富，你可以在控制台输入 console。  

7. 	变量是一个名称。字面量是一个值。  

8. JavaScript 中，常见的是驼峰法的命名规则，如 lastName (而不是lastname)。  

9. JavaScript 是脚本语言。浏览器会在读取代码时，逐行地执行脚本代码。而对于传统编程来说，会在执行前对所有代码进行编译。  

10. 反斜杠换行  
    document.write("你好 \ W3Cschool!");  

11. 一个好的编程习惯是，在代码开始处，统一对需要的变量进行声明。

12. 你的全局变量，或者函数，可以覆盖 window 对象的变量或者函数。 
局部变量，包括 window 对象可以覆盖全局变量和函数。

13. 在 ES6 中，提供了 let 关键字和 const 关键字。
    let 的声明方式与 var 相同，用 let 来代替 var 来声明变量，就可以把变量限制在当前代码块中。
    使用 const 声明的是常量，其值一旦被设定便不可被更改。














