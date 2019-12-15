# JS-常见报错

```js
	// js代码出现报错后，程序就不执行了
    //  - 了解常见的报错含义和常用，有助于我们解决问题

    // 1 引用错误  ReferenceError
    //   形式： Uncaught ReferenceError: xxx is not defined
    //    - Uncaught 未捕获
    //    - Reference 引用，使用
    //    - Error 错误
    //    - defined 定义

    //   常见出现场景：变量或函数名写错了

    // 2 类型错误  TypeError
    //   形式：
    //     Uncaught TypeError: Cannot read property 'xxxx' of null
    //     Uncaught TypeError: xxx is not a function
    //       - property 属性(方法)
    //       - read 读取

    //   常见的出现场景：对某个值的使用方式不符合类型本身的功能
    //     - null和undefined不具有属性，如果进行属性访问会报错
    //       - 获取了数组不存在的元素后，又进行属性访问等操作...
    /*
    var arr = [1, 2, 3];
    arr[0].toString();
    arr[4].toString(); // 错误的访问的元素，导致报错
     */
    /*
    var box = document.getElementById('box2'); // null
    box.innerHTML = 'abc'; // 错误的获取了元素，导致报错
    */

    /*
    var obj = {
      sayHi: function () {
        console.log('我是obj，你好啊');
      }
    };
    obj.sayHi();
    obj.sayhi(); // 错误的方法名拼写导致错误
     */

    // 3 语法错误  SyntaxError
    //  通常vscode编辑器会直接提示错误，不需要自己单独分析查找
    //  形式：
    //    Uncaught SyntaxError: Unexpected token ')'
    //    Uncaught SyntaxError: missing ) after argument list
    //    - Syntax 语法
    //    - Unexpected 不期待的
    //    - token 标识符
    //      - 变量名，函数名，属性名，方法名..

    //  常见的出现场景：各种语法拼错了，导致的错误(缺少括号，或者括号太多套错了)
```

