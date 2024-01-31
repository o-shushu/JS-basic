### 一.形式/注释/输出
* 内嵌JS
* 行内式JS
* 外部JS
* 单行注释
* 多行注释
* 浏览器弹出输入框，用户可以输入
* 浏览器控制台打印输出信息
* 浏览器弹出警示框

#### 内嵌JS
```html
   <script>
        alert('hi!World')
   </script>
```
#### 行内式JS
```html
   <input type="button" value="click me" onclick="alert('hello world')"/>
```
#### 外部JS
```html
   <script src="sample.js"></script>
```
#### 单行注释
```html
   <script>
    //输出内容
    // 多行注释快捷键：ctrl+/
        alert('hi!World')
   </script>
```
#### 多行注释
```html
   <script>
    /* 输入输出语句之浏览器弹出警示框
    多行注释快捷键：alt+shift+a */
        alert('hi!World')
   </script>
```
#### 浏览器弹出输入框，用户可以输入
```html
    <script>
        prompt();//来自prompt()的值是字符串型
    </script>
```
#### 浏览器控制台打印输出信息
```html
    <script>
        console.log();//显示给程序员自己看
    </script>
```
#### 浏览器弹出警示框
```html
    <script>
        alert();//显示给用户看
    </script>
```

### 二.变量使用
* 声明
* 赋值
* 变量的初始化
* 案列测试
    * 我叫Jane，我住在上海，我今年 30 岁了，我的邮箱是 Jane@test.cn，我的工资 20k/月
    * 弹出一个输入框，提示用户输入姓名。
    * 弹出一个对话框，输出用户刚才输入的姓名。
* 赋值覆盖
* 声明多个变量
* 声明变量的（）种特殊情况
* 变量命名规范
    * （  ）大小写；不能以（  ）开头；（  ）不能作为变量名
由（  ）（ ）（ ）（ ）组成；遵守（  ）命名法；
* 变量练习
    * 交换两个变量的值
#### 声明
```html
    <script>
        var color//用var来声明变量
    </script>
```
#### 赋值
```html
    <script>
        var color;
        color = "blue";
    </script>
```
#### 变量的初始化
```html
    <script>
        var age = 18;
    </script>
```
#### 案列测试
```html
    <script>
        var name = "Jane";
        var add = "上海";
        var age = 30;
        var email = "Jane@test.cn";
        var salary = 20000;
        var fname = prompt();
        alert(fname);
    </script>
```
#### 赋值覆盖
```html
    <script>
        var age = 18;
        age = 28;
        console.log(age);
    </script>
```
#### 声明多个变量
```html
    <script>
        var name = "Jane", add = "上海", age = 30;
    </script>
```
#### 声明变量的（3）种特殊情况
```html
    <script>
        //1.只声明不赋值
        var name
        console.log(name);//undefined
        //2.未声明未赋值
        console.log(age);//error
        //3.未声明有赋值,不提倡使用
        age = 17;
        console.log(age);//17
    </script>
```
#### 变量命名规范
（ 严格区分 ）大小写；
不能以（ 数字 ）开头；
（ 关键字，保留名 ）不能作为变量名;
由（ 字母 ）（数字 ）（ 下划线_）（美元符号$ ）组成；
遵守（ 驼峰 ）命名法；
#### 变量练习
```html
    <script>
        var num1 = 6, num2 = 8;
        var num3;
        num3 = num1;
        num1 = num2;
        num2 = num3;
        console.log(num1, num2);
    </script>
```

### 三.数据类型
* 理论概述
    * 因数据占用（）不同，为充分利用（）而划分不同数据类型
    * JavaScript是一种（）语言，也是（）语言
    * 变量的数据类型取决于（）
    * 相同的变量可以用作（）
    * JS的数据类型可以分为（）种，分别是
        * （）:包含（）（）（）（）（）
        * （）:包含（）
* 简单数据类型
    * 数字型
        * 包含（）值和（）值
        * 数字型进制:在JS中，八进制前面加（）范围（），十六进制前面加（）范围（）
        * 最大值:(),最小值:()
        * 三个特殊值（无穷大:()/无穷小:()/NaN表示（））
        * isNaN()作用:（）
    * 字符串类型
        * 外双内单，外单内双
        * 转义符需加（）开头，要写到（）里
        * 字符串长度:()
        * 字符串拼接用（）符号，（）相加，（）相连
        * 显示年龄案列
            * 弹出一个输入框，需要用户输入年龄，之后弹出一个警示框显示“您今年 xx 岁啦”（ xx 表示刚才输入的年龄）
    * 布尔类型
        * 只有（）个值，分别为（）相当于数字（），（）相当于数字（）
    * 未定义
        * undefined和数字相加，最后的结果是（）
    * 空值
        * null空值，表示（）
* 复杂数据类型
* 获取变量数据类型:()
* 数据类型转换
    * 转为字符串:3种方式
    * 转为数字型:4种方式
    * 计算年龄案例
    * 简单加法器案例
    * 转为布尔型:1种方式
* 扩展
#### 理论概述
    * 因数据占用（存储空间）不同，为充分利用（存储空间）而划分不同数据类型
    * JavaScript是一种（弱类型或者说是动态）语言，也是（编程）语言
    * 变量的数据类型取决于（变量值的数据类型来判断）
    * 相同的变量可以用作（不同的类型）
    * JS的数据类型可以分为（2）种，分别是
        * （简单数据类型）:包含（number）（string）（boolean）（undefined）（null）
        * （复杂数据类型）:包含（object）
#### 简单数据类型
##### 数字型
* 包含（整型）值和（浮点型）值
```html
    <script>
        var num1 = 18;
        var num2 = 3.14;
    </script>
```
* 数字型进制:在JS中，八进制前面加（0）范围（0~7），十六进制前面加（0x）范围（0~9及A~F）
```html
    <script>
        var num1 = 07;
        var num2 = 08;
        var num3 = 0xB;
    </script>
```
* 最大值:(Number.MAX_VALUE),最小值:(Number.MIN_VALUE)
```html
    <script>
        alert(Number.MAX_VALUE);
        alert(Number.MIN_VALUE);
    </script>
```
* 三个特殊值（无穷大:(Infinity)/无穷小:(-Infinity)/NaN表示（非数字））
```html
    <script>
        alert(Infinity);
        alert(-Infinity);
        alert(NaN);
    </script>
```
* isNaN()作用:判断变量是否为非数字的类型
```html
    <script>
        var age = 18;
        var content = "1周有7天"
        var result1 = isNaN(age);
        var result2 = isNaN(content);
        console,log(result1);//false
        console,log(result2);//true
    </script>
```
##### 字符串类型
* 外双内单，外单内双
```html
    <script>
        var message1 = "麻辣烫，'不要麻'，不要辣，只要烫";
        var message2 = '麻辣烫，"不要麻"，不要辣，只要烫';
        console,log(message1);
        console,log(message2);
    </script>
```
* 转义符需加（\）开头，要写到（引号）里
```html
    <script>
        alert('酷热难耐，火辣的太阳底下，我挺拔的身姿，成为了最为独特的风景。\n我审视四周，这里，是我的舞台，我就是天地间的王者。\n这一刻，我豪气冲天，终于大喊一声： " 收破烂啦～ "');
    </script>
```
* 字符串长度:(length)
```html
    <script>
        var message = "麻辣烫，'不要麻'，不要辣，只要烫";
        alert(message.length);
    </script>
```
* 字符串拼接用（+）符号，（数字）相加，（符号）相连
```html
    <script>
        alert('message' + 'length');
        alert('110' + 110);
        alert('110' + '110');
    </script>
```
* 显示年龄案列
    弹出一个输入框，需要用户输入年龄，之后弹出一个警示框显示“您今年 xx 岁啦”（ xx 表示刚才输入的年龄）
```html
    <script>
        var age = prompt();
        var message = "您今年已经" + age + "岁了";
        alert(message);
    </script>
```  
##### 布尔类型
* 只有（2）个值，分别为（true）相当于数字（1），（false）相当于数字（0）
```html
    <script>
        console.log(true + 1);
        console.log(false + 1);
    </script>
```  
##### 未定义
* undefined和数字相加，最后的结果是（NaN
```html
    <script>
        var variable;
        console.log(variable + 18);
    </script>
```
##### 空值
* null空值，表示（什么都没有）
```html
    <script>
        var variable = null;
        console.log(variable + 18);//18
        console.log(variable + true);//1
    </script>
```
#### 获取变量数据类型:(typeof)
```html
    <script>
        var num = 18;
        var text = "happy";
        var bool = true;
        var variable = null;
        var who;
        var num1 = prompt()//来自prompt()的值是字符串型
        console.log(typeof num);
        console.log(typeof text);
        console.log(typeof bool);
        console.log(typeof variable);
        console.log(typeof who);
        console.log(typeof num1);
    </script>
```
#### 数据类型转换
* 转为字符串:3种方式
```html
     <script>
        var num = 68;
        console.log(num.toString());
        console.log(String(num));
        console.log(num + '');
    </script>
```
* 转为数字型:4种方式
```html
    <script>
        var text = "18.99";
        var result = text - 0
        console.log(parseInt(text), typeof parseInt(text));//得到的是整数，会去掉单位
        console.log(parseFloat(text), typeof parseFloat(text));//得到的是浮点数
        console.log(Number(text), typeof Number(text));
        console.log(result, typeof result);//利用算术运算- * /
    </script>
```
* 计算年龄案例
```html
    <script>
        var year = prompt("请输入您的出生年份");
        var age = 2024 - year;
        var result = "您今年" + age + "岁了";
        alert(result)  
    </script>
```
* 简单加法器案例
```html
<script>
    var num1 = prompt("请输入第一个数");
    var num2 = prompt("请输入第二个数");
    var result = Number(num1) + Number(num2);
    alert("结果是" + result); 
</script>
```
* 转换为布尔型:1种方式（Boolean()）
代表空、否定的值会被转换为 false ，如 '' 、 0 、 NaN 、 null 、 undefined
```html
<script>
    console.log(Boolean(''));
    console.log(Boolean(0));
    console.log(Boolean(NaN));
    console.log(Boolean(null));
    console.log(Boolean(undefined));
</script>
```
#### 扩展
* 翻译器：将程序语言翻译成机器语言的工具。
* 解释型语言：边解释边执行（JS）
* 编译型语言：全部解释完后再执行(Java)
* 标识符：开发人员为变量，属，函数，参数取的名字。标识符不能是关键字或保留字。
* 关键字：JS本身已经使用的字不能再作为变量名，方法名。
* 保留字：预留的关键字，未来可能成为关键字的名。
* 练习
    * 依次询问并获取用户的姓名、年龄、性别，并打印用户信息如图
```html
<script>
    var username = prompt("请输入您的名字：");
    var age = prompt("请输入您的年龄：");
    var sex = prompt("请输入您的性别：");
    alert('结果是:\n姓名:'+ username + '\n年龄:' + age + '\n性别:' + sex);
</script>
```

### 四.JS运算符p41




