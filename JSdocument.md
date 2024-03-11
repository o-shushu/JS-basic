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
* undefined和数字相加，最后的结果是（NaN）
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

### 四.JS运算符
* 算术运算符
    * 加减乘除，取余
    * 浮点数精度问题
    * 如何判断一个数能够被整除
    * 表达式由（）（）（）等组成的式子
* 递增/递减运算符
    * 前置递增
    * 后置递增
    * 练习
* 比较运算符
    * (<,>,>=,<=,==,!=,===)
* 逻辑运算符
    * 短路运算（逻辑中断）之与
    * 短路运算（逻辑中断）之或
* 赋值运算符
* 优先级运算符
#### 算术运算符
* 加减乘除，取余
* 浮点数精度问题
```html
<script>
    console.log(1 + 1);
    console.log(1 - 1);
    console.log(1 * 1);
    console.log(1 / 1);
    //取余（取模）
    console.log(4 % 2);
    console.log(3 % 5);
    //浮点数的算数运算时会有精度问题,不能直接拿浮点数进行比较
    var result = 0.1 + 0.2;
    console.log(result);//结果不等于0.3
</script>
```
* 如何判断一个数能够被整除:余数为0就能被整除
```html
<script>
    console.log(4 % 2);
</script>
```
* 表达式由（数字）（运算符）（变量）等组成的式子.表达式最终会返回一个结果（返回值）
#### 递增/递减运算符
前置递增and后置递增:两者单独使用一样,和其他代码联用时，执行结果不同
 * 前置递增:先自加，后返回值 ++age
```html
<script>
    var num = 10;
    console.log(++num + 10);//21; num = num + 1, num = 11, ++num = 11
</script>
```
* 后置递增:先表达式返回原值，后num这个变量自加1 num++
```html
<script>
    var num = 10;
    console.log(10 + num++);//20; num++ = 10, num = 11
</script>
```
* 练习
```html
<script>
    var a = 10;
    ++a;
    var b = ++a + 2;
    console.log(b);//14

    var c = 10;
    c++;
    var d = c++ + 2;
    console.log(d);//13

    var e = 10;
    var f = e++ + ++e;//e++ = 10 e = 11; ++e = 12
    console.log(f);//22
</script>
```
#### 比较运算符
* (<,>,>=,<=,==[判断号],!=,===[全等号])
比较后，返回布尔值
```html
<script>
    console.log(18 == '18');//true
    console.log(18 != 18);//false
    //全等于===，值及数据类型都一致
    console.log(18 === '18');//false

    var num1 = 10;
    var num2 = 100;
    var rea1 = num1 > num2;
    var rea2 = num1 == 11;
    var rea3 = num1 != num2;
    console.log(rea1);//false
    console.log(rea2);//false
    console.log(rea3);//true
</script>
```
#### 逻辑运算符
多个条件判断，进行布尔值运算的运算，返回值为布尔值
* &&  逻辑与
* ||  逻辑或
* !   逻辑非
```html
<script>
    console.log(3 > 5 && 3 > 2);//false
    console.log(3 > 5 || 3 > 2);//true
    console.log(!true);//false
    //practice
    var num = 7;
    var str = "peace and love";
    console.log(str.length);//12 长度为14，空格也算
    console.log(num > 5 && str.length >= num);//true
    console.log(num < 5 && str.length >= num);//false
    console.log(!(num < 10));//false
    console.log(!(num < 10 || str.length == num));//false
</script>
```
* 短路运算（逻辑中断）之与
如果第一个表达式1为真，则返回表达式2
如果第一个表达式1为假，则返回表达式1
```html
<script>
    console.log(123 && 456);//456
    console.log(0 && 456);//0
    console.log(0 && 1 + 2 && 456 * 56789);//0
    //如果有空的或者否定的则为假，其余为真
    //0 '' null undefined NaN
    console.log(null && 456);//null
    console.log('' && 456);//
    console.log(undefined && 456);//undefined
    console.log(NaN && 456);//NaN
</script>
```
* 短路运算（逻辑中断）之或
如果第一个表达式1为真，则返回表达式1
如果第一个表达式1为假，则返回表达式2
```html
<script>
    console.log(123 || 456);//123
    console.log(0 || 456 || 456 + 123);//456

    var num = 0;
    console.log(123 || num++);
    console.log(num);//0
</script>
```
#### 赋值运算符
右边值给左边
```html
<script>
    var num = 10;
    num += 2;
    console.log(num);//12
    num += 5;
    console.log(num);//17
    num -= 2;
    console.log(num);//15
</script>
```
#### 优先级运算符
优先级从高到低排列
* ()
* [++,--,!] 有一个变量操作运算的为一元运算符
* [*/%+-]
* [>, >=, <, <=]
* [==, !=, ===, !==]
* [&&, ||]
* [=]
* [,]

### 五.JS流程控制
* 流程控制
    * 顺序结构
    * 分支结构
        * if语句
        * if else语句
        * 判断闰年
        * 判断是否中将
        * if else if语句
        * 判断成绩
        * switch语句
        * 查询水果（案例）
        * switch语句和if else if语句的区别
            * 案例练习（见PPT）
    * 循环结构
        * 循环的目的
        * for循环（可以重复执行相同代码和不同代码）
        * 断点调试观察代码
        * 累加求和案例
        * 求1~100间（平均值，偶数和奇数的和，能被3整除数字的和）
        * 求学生成绩案例
        * 一行打印5颗星星案例
        * 双重for循环+案例
        * while循环和do while循环
        * break和continue区别
        * 循环作业（题目见PPT）
* 三元表达式
    * 语法结构
    * 数字补0（案例）
        * 用户输入数字，如果数字小于 10 ，则在前面补 0 ，比如 01 ， 09 ，如果数字大于 10 ，则不需要补，比如
20 。
#### 流程控制
有（3）种结构，分别是（顺序）结构，（分支）结构，（循环）结构。
* 顺序结构
* 分支结构(根据条件选择，多选一)
    * if语句
    ```html
    <script>
        // 条件成立执行代码，否则什么也不做
        if ( 条件表达式 ) {
        // 条件成立执行的代码语句
        }
    </script>
    ```
    * if else语句
    ```html
        <script>
            // 条件成立 执行 if 里面代码，否则执行 else 里面的代码
            if ( 条件表达式 ) {
            // [ 如果 ] 条件成立执行的代码
            } else {
            // [ 否则 ] 执行的代码
            }
        </script>
    ```
    * 判断闰年
    ```html
    <script>
        var year = prompt("请输入年份：");
        if(year % 4 == 0 && year % 100 != 0 || year % 400 == 0) {
            alert(year + "是闰年");
            console.log(year % 2);
        }else {
            alert(year + "是平年");
            console.log(year % 2);
        }
    </script>
    ```
    * 判断是否中奖
    ```html
    <script>
        var username = prompt("请输入您的姓名：");
        if(username == "刘德华") {
            alert("恭喜中了5元!");
        } else {
            alert("非常遗憾，您没有中奖!");
        }
    </script>
    ```
    * if else if语句
    ```html
    <script>
        if (条件表达式1) {
            // 条件成立执行的代码语句
        } else if (条件表达式2) {
            // 条件成立执行的代码语句
        } else if (条件表达式3) {
            // 条件成立执行的代码语句
        } else {
            // 条件成立执行的代码语句
        }
    </script>
    ```
    * 判断成绩
    ```html
    <script>
         if (score >= 90) {
            alert("A");
        } else if (score >= 80) {
            alert("B");
        } else if (score >= 70) {
            alert("C");
        } else if (score >= 60) {
            alert("D");
        } else {
            alert("E");
        }
    </script>
    ```
    * switch语句
        * 表达式返回的值是否有满足case中的value，有就执行相应语句，都没有就执行default下的语句。
        * 注：表达式返回的值和case的值必须全等（值和数据类型一致）
    ```html
    <script>
      switch(表达式) {
        case value1:
            执行的代码语句;
            break;//break表退出，若没有就会继续执行下一个case
        case value2:
            执行的代码语句;
            break;
        ...
        default:
            执行最后的语句;   

      }  
    </script>
    ```
    * 查询水果（案例）
     ```html
    <script>
      var input = prompt("请输入要查询的水果：");
        switch(input) {
            case "苹果":
                alert("2.5元/斤");
                break;
            case "草莓":
                alert("25元/斤");
                break;
            case "香蕉":
                alert("3元/斤");
                break;
            default:
                alert("没有此水果");
        }
    </script>
    ```
    * switch语句和if else if语句的区别
        * 一般情况下可以互相替换
        * switch语句处理固定值，if else if语句用于范围判断
        * 分支较多时，switch语句效率高；分支较少时，if...else语句效率较高
* 循环结构
   * 循环的目的：可以重复执行某些代码/语句
   * for循环
        * 循环体：被重复执行的语句
        * 终止条件：能否继续重复执行的条件
        * 初始化变量: 声明的一个普通变量，作为计数器使用
        * 条件表达式（终止条件）:判断循环是否继续执行
        * 操作表达式:每次循环最后执行的代码，用于计数器的更新
        ```html
            <script>
                for (初始化变量;条件表达式;操作表达式) {
                    //循环体
                }

            //如：
            for (var i = 1; i <= 100; i++) {
                console.log("How are you?");
            }
            </script>
        ```
   * 断点调试观察代码
        * 目的：观察程序的运行过程
        * 流程：F12->Sources(Page)->指定要调试的行号，再刷新页面（浅蓝色背景在哪里就到哪一步）->F11（watch用于监视变量的值的变化）
   * 累加求和案例
   ```html
    <script>
        for (var i = 1, sum = 0; i <= 100; i++) {
            sum = sum + i;//sum += i
        }
        console.log(sum);
    </script>
   ```
   * 求1~100间（平均值，偶数和奇数的和，能被3整除数字的和）
   ```html
    <script>
        var sum = 0;
        var average = 0;
        for (var i = 1; i <= 100; i++) {
            sum = sum + i;
        }
        average = sum / 100;
        console.log(average);

        var even = 0;
        var odd = 0;
        for (var i = 1; i <= 100; i++) {
            if (i % 2 == 0) {
                even = even + i;
            } else {
                odd = odd + i;
            }
        }
        console.log(even);
        console.log(odd);

        var three = 0;
        for (var i = 1; i <= 100; i++) {
            if (i % 3 == 0){
                three = three + i;
            }
        }
        console.log(three);
    </script>
   ```
   * 求学生成绩案例
   ```html
    <script>
        var total = 0;
        var score;
        var num = prompt("请输入学生人数：");
        for (var i = 1; i <= num; i++) {
        score = prompt("请输入学生" + i + "的成绩：");
        total = total + Number(score);
        }
        average = total / Number(num);
        alert("学生的平均成绩：" + average);
    </script>
   ```
   * 一行打印5颗星星案例
   ```html
    <script>
        var total = "";
        for (var i = 1; i <= 5; i++) {
            star = '*';
            var total = total + star;
        }
        console.log(total);
    </script>
   ```
   * 双重for循环+乘法表案例
        * 语法结构:外层执行1次，里层的循环要全部执行
        ```html
        <script>
            for (外层的初始化变量；外层的条件表达式；外层的操作表达式) {
                for (里层的初始化变量；里层的条件表达式；里层的操作表达式) {
                    //执行语句
                }
            }
        </script>
        ```
        * 案例
        ```html
        <script>
        //打印5行5列星星案例
            var stars = '';   
            for (var i = 1; i <= 5; i++) {
                for (var j = 1; j <= 5; j++) {
                    stars = stars + '*';
                }
                stars = stars + '\n';
            }
            console.log(stars);
        //自定义行列星星案例
            var stars = '';
            var rows = prompt('请输入行数：');
            var columns = prompt('请输入列数：');

            for (var i = 1; i <= rows; i++) {
                for (var j = 1; j <= columns; j++) {
                    stars = stars + '*';
                }
                stars = stars + '\n';
            }
            console.log(stars);
        //打印倒三角案例n行
            var stars = '';
            var num = prompt('请输入行数：');
            for (var i = 1; i <= num; i++) {
                for (var j = 1; j <= num - i + 1; j++) {
                    stars = stars + '*';
                }
                // for (var j = i; j <= num; j++) {
                //     stars = stars + '*';
                // }
                stars = stars + '\n';
            }
            console.log(stars);
        //打印正三角案例n行
            var stars = '';
            var num = prompt('请输入行数：');
            for (var i = 1; i <= num; i++) {
                for (var j = 1; j <= i; j++) {
                    stars = stars +'*';
                }
                stars = stars + '\n';
            }
            console.log(stars);
        //九九乘法表案例
            var cows = prompt('请输入行数：');
            var results = '';
            for (var i = 1; i <= cows; i++) {
                for (var j = 1; j <= i; j++) {
                    var product = j * i;
                    var results = results + '\t' + j + 'x' + i + '=' + product;
                }
                results += '\n';
            }
            console.log(results);
        </script>
        ```
   * while循环和do while循环
        * while循环:条件表达式为真时，执行循环体;可以用于更复杂的循环
        ```html
        <script>
            while (条件表达式) {
                //循环体
            }
        //案例1
            var i = 1;
            var sum = 0;
            while (i <= 100) {
                sum = sum + i;
                i++
            }
            console.log(sum);
        //案例2
        var message = prompt('今天谁请客呀？');
        while (message != '我请客')  {
            message = prompt('今天谁请客呀？');
        }
        alert('多谢款待');
        </script>
        ```
        * do while循环:先执行循环体，再判断，符合条件就退出
        ```html
        <script>
            do {
                //循环体
            } while (条件表达式)
        </script>
        ```
        * 案例
        ```html
        <script>
            var age = 1;
            do {
                console.log('我今年'+ age +'岁了!');
                age++;
            } while (age <= 100)
        </script>
         ```
   * break和continue区别
        * continue:只是跳出本次循环，继续下一次循环
        ```html
        <script>
            for (var i = 1; i <= 5; i++) {
                if (i == 3) {
                    continue;
                }
                console.log('我正在吃第'+ i +'个面包');
            }

            var sum = 0;
            for (var i = 1; i <= 100; i++) {
                if (i % 7 == 0) {
                    continue;
                }
                sum += i;
            }
            console.log(sum);
        </script>
        ```
        * break:结束整个循环,后面的不再执行
        ```html
        <script>
            for (var i = 1; i <= 5; i++) {
                if (i == 3) {
                    break;
                }
                console.log('我正在吃第'+ i +'个面包');
            }
        </script>
        ```
   * 循环作业（题目见PPT）
#### 三元表达式
* 语法结构
    条件表达式 ? 表达式1 : 表达式2
    ```html
    <script>
        var num = 8;
        var result = num > 5 ? "true" : "false"; 
        console.log(result);
    </script>
    ```
* 数字补0（案例）
    ```html
    <script>
        var num = prompt("请输入数字：");
        var result = num < 10 ? "0" + num : num;
        console.log(result);
    </script>
    ```

### 六.数组
* 为什么要有数组
* 创建数组
    * 创建方式
* 获取数组中的元素
    * 数组的索引
    * 访问元素的格式
* 对数组进行遍历
    * 遍历数据
    * 数组的长度
    * 求数组元素的和及平均值
    * 求数组最大值/最小值
    * 数组转化为分割字符串
* 给数组新增元素
    * 新增元素方法(修改长度length;修改索引号)
    * 新建一个数组里面存放1~10的元素
    * 案例
        * 选数新建一个数组
        * 删除指定数组元素
        * 翻转数组
* 冒泡排序案例
#### 为什么要有数组
* 数组：一组数据的集合,可放任意数据类型，用逗号分隔，里面的数据称为数组元素
* 作用：将一组数用一个变量表示
#### 创建数组
* 创建方式
    * （1）利用new
    ```html
    <script>
        var arr = new Array();
    </script>
    ```
    * （2）数组字面量
    ```html
    <script>
        var arr = [1, 2, 3, 4]
    </script>
    ```
#### 获取数组中的元素
* 数组的索引：数组元素的序号
* 访问元素的格式：数组名[索引号],索引号从0开始
    ```html
    <script>
        var arr = [1, 2, 3, 4]
        console.log(arr[1]);
    </script>
    ```
#### 对数组进行遍历
* 遍历数据：将数组中的每个元素从头到尾都访问一遍
    ```html
    <script>
        var arr = ["red", "blue", "green", "black"]
        for (var i = 0; i < 4; i++) {
            console.log(arr[i]);
        }
    </script>
    ```
* 数组的长度：数组名.length,其长度是数组的个数
    ```html
    <script>
        var arr = ["red", "blue", "green", "black"]
        for (var i = 0; i < arr.length; i++) {
            console.log(arr[i]);
        }
    </script>
    ```
* 求数组元素的和及平均值
    ```html
    <script>
        var arr1 = [2, 6, 1, 7, 4];
        var sum = 0;
        for (var i = 0; i < arr1.length; i++) {
            sum = sum + arr1[i];
        }
        console.log(sum);
        console.log(sum / arr1.length);
    </script>
    ```
* 求数组最大值/最小值
    ```html
    <script>
        var arr2 = [2, 6, 1, 77, 52, 25, 7, 100];
        var i = 0;
        var max = arr2[i];
        do {
            if (arr2[i] > max) {
                max = arr2[i];
            }
            i++
        } while (i < arr2.length)
        console.log(max);

        var min = arr2[0];
        for (var i = 1; i < arr2.length; i++) {
            if (min - arr2[i] >= 0) {
                min = arr2[i];
            }
        }
        console.log(min);
    </script>
    ```
* 数组转化为分割字符串
    ```html
    <script>
        var arr = ["red", "blue", "green", "black"];
        var new_arr = '';
        var sep = '|';
        for (var i = 0; i < arr.length; i++) {
            var element = arr[i] + sep;
            new_arr =  new_arr + element;
        }
        console.log(new_arr);
    </script>
    ```
#### 给数组新增元素
* 新增元素方法：2种
* 数组中新增元素不能直接给数组赋值，否则会被覆盖
    ```html
    <script>
        //修改长度length新增
        var arr = ["red", "blue", "green", "black"];
        arr.length = 6;
        console.log(arr);
        console.log(arr[4]);
        console.log(arr[5]);
        //修改索引号新增
        var arr1 = ["red", "blue", "green", "black"];
        arr1[4] = "pink";
        console.log(arr1);
    </script>
    ```
* 新建一个数组里面存放1~10的元素
    ```html
    <script>
        var num_arr = [];
        for (var i = 0; i < 10; i++) {
            num_arr[i]= i +1;

        }
        console.log(num_arr);
    </script>
    ```
* 案例
    * 选数新建一个数组。还有另一种采用new_arr[new_arr.length]的方法
    ```html
        <script>
            var new_arr = [];
            var old_arr = [2, 6, 1, 77, 52, 25, 7, 100];
            for (var i = 0, j = 0; i < old_arr.length; i++) {
                if (old_arr[i] >= 10) {  
                    new_arr[j] = old_arr[i];
                    j++;
                }
            }
            console.log(new_arr); 
        </script>  
    ```
    * 删除指定数组元素
    ```html
        <script>
            var old_arr = [2,0,6,1,77,0,52,0,25,7];
            var newArr = [];
            for (var i = 0; i < old_arr.length; i++) {
                if (old_arr[i] != 0) {  
                    newArr[newArr.length] = old_arr[i];
                }
            }
            console.log(newArr);
        </script>  
    ```
    * 翻转数组
    ```html
        <script>
            var col_arr = ["red","green","blue","pink","purple"];
            var turn_arr = [];
            for (var i = 0; i < col_arr.length; i++) {
                turn_arr[col_arr.length-1-i] = col_arr[i];
            }
            console.log(turn_arr);
        </script>  
    ```
* 冒泡排序：一种算法，将一系列数据按一定顺序排列显示（从大到小或从小到大）
    * 注意每次是两位数进行比较
   ```html
    <script>
        var arr = [5,4,3,2,1,8,10,9];
        for (var i = 0; i < arr.length; i++) {  
            for (var j = 0; j < arr.length - i - 1; j++) {
                    if (arr[j] > arr[j + 1]) {
                        var temp = arr[j];
                        arr[j] = arr[j + 1];
                        arr[j + 1] = temp;
                        
                    }
                }
        };
        console.log(arr);
    </script>
    ```


### 七.JS函数
* 为什么需要函数
    * 概念
    * 使用
        * 声明函数
    * 参数
        * 形参
        * 实参
        * 执行过程
        * 形参和实参个数不匹配
* 使用函数的返回值
* arguments获取函数的参数
    * 案例
* 函数的相互调用
* 函数的声明方式
#### 为什么需要函数
* 概念：封装一段可以重复执行的代码
    ```html
        <script>
            //求10~50的累加和
                /* var sum = 0;
                for (sum1 = 10; sum1 <= 50; sum1++) {
                    sum += sum1;
                }
                console.log(sum); */
                //求50~100,40~80等的累加和,使用JS的函数更高效
                function getSum(sum1, sum2) {
                    var sum = 0;
                    for (var i = sum1; i <= sum2; i++) {
                        sum += i;
                    }
                    console.log(sum);
                }
                getSum(1, 100);
                getSum(10, 50);
                getSum(1, 1000);
                getSum(40, 80);
        </script>
    ```
* 使用
    * 声明函数
    ```html
    <script>
        function 函数名() {
            函数体
        }
    </script>
    ```
    function：关键字，必须小写
    函数名：一般是动词
    函数不调用不执行
    * 调用函数
        函数名()
* 参数：利用函数参数实现函数重复不同的代码
    * 形参：形式上的参数
        ```html
            <script>
                function 函数名(形参1，形参2...) {
                    函数体
                }
            </script>
        ```
    * 实参：实际的参数
        函数名(实参1，实参2...)
    * 执行过程
        函数的参数可有可无,形参不用声明
        ```html
            <script>
                function cook(sub) {
                    console.log(sub);
                }
                cook('apple');
            </script>
        ```
    * 形参和实参个数不匹配
        ```html
            //形参个数 > 实参个数  ==> 正常计算
            //形参个数 < 实参个数  ==>  NaN
        ```
#### 使用函数的返回值
不能将结果返回给函数内部，应该返回给函数调用者
```html
    <script>
        function 函数名(形参1，形参2...) {
            return 需要返回的结果
        }

        function cook(sub) {
            return sub;
        }
        console.log(cook('apple'));

    </script>
```
* 案例
利用函数求两个数的最大值
```html
    <script>
        function getMax(sum1, sum2) {
            /* if (sum1 > sum2) {
                return sum1;
            } else {
                return sum2;
            } */
            result = num1 > num2 ? num1 : num2;
            return result;
        }
        console.log(getMax(323, 543));
    </script>
```
//求任意数组的最大值
```html
    <script>
        function getArrMax(arr) {
            var max = arr[0];
            for(var i = 1; i < arr.length; i++) {
                if (arr[i] > max) {
                    max = arr[i];
                }
            }
            return max;
        }

        var result = getArrMax([12, 3, 4, 76, 21, 88]);
        console.log(result);
    </script>
```
* return终止函数：后面代码不会执行；只能返回1个值且是最后一个值 
#### arguments的使用
*  arguments:存储了传递的所有实参；展示为伪数组形式；每个函数都内置好的
* 伪数组：不是真正意义上的数组；具有length属性；按照索引方式进行存储；没有真正数组的一些方法pop(),push()
```html
    <script>
        function fn() {
        console.log(arguments);
        }

        fn(1, 2, 3);
        
    </script>
```
//利用函数求任意个数的最大值
```html
    <script>
        function getMax() {
            var max = arguments[0];
            for(var i = 1; i <arguments.length; i++){
                if(arguments[i] > max) {
                    max = arguments[i]
                }
            }
            return max;
        }
        console.log(getMax(43, 23, 5, 67, 33, 45));
    </script>
```
//利用函数翻转数组
```html
<script>
    function list(arrList) {
        for(var i = 0, List = []; i < arrList.length; i++){
            
            List[i] = arrList[arrList.length - i -1];
        }
        return List;
    }
    console.log(list([12, 3, 4, 76, 21, 88]));
    console.log(list(['red', 'black','white']));
</script>
```
//利用函数进行冒泡排序#&%
```html
    <script>
        function sort(group) {
            for(var i = 0; i < group.length; i++){
                for(var j = 0; j < group.length - i - 1; j++){
                    if(group[j] > group[j + 1]){
                        var temp = group[j];
                        group[j] = group[j + 1];
                        group[j + 1] = temp;
                    }
                }
            }
            return group;
        }
        console.log(sort([12, 3, 4, 76, 21, 88])); 
    </script>
```
//利用函数判断闰年
```html
    <script>
        function yearIs(year){
            if(year % 4 == 0 && year % 100 != 0 || year % 400 == 0){
                return year + "是闰年";
            } else {
                return year + "不是闰年";
            }
        }
        console.log(yearIs(2000));
        console.log(yearIs(1999));  
    </script>
```
#### 函数的相互调用
    ```html
    <script>
            function yearIs(year){
            if(year % 4 == 0 && year % 100 != 0 || year % 400 == 0){
                return true;
            } else {
                return false;
            }
        }
        console.log(yearIs(2000));
        console.log(yearIs(1999));
    //用户输入年份，并输出当前年份2月份的天数
        function backDay(){
            var year = prompt('请输入年份：');
            if(yearIs(year)){
                alert('当前年份是闰年2月份有29天');
            } else {
                alert('当前年份是平年2月份有28天');
            }
        }
        backDay();
    </script>
    ```
#### 函数的声明方式
    ```html
    <script>
        //1.命名函数。利用关键字
        function fn() {

        }
        fn();

        //2.匿名函数（函数表达式）
        var 变量名= function(){};
        var as = function(){

        }
        as();

        //as是变量名，不是函数值
        //函数表达式里面存的是函数
        //函数表达式也可以传递参数
        
    </script>
    ```

### 八.JS作用域
* 作用域：代码名字在某个范围内起作用和效果。目的是为了提高程序的可靠性，减少命名冲突。
    * ecma（es）的script标准，用最多es5。在es6时新增块级作用域{},外面是不能使用里面的变量
* 全局作用域：整个script标签
* 局部作用域（函数作用域）：只在函数内部起作用
* 全局变量：在全局作用域下的变量；在函数内部没有直接声明就赋值的变量
* 局部变量（函数作用域）：只在函数内部起作用;函数的形参
* 执行效率
    全局变量只有浏览器关闭时才会销毁，占内存资源。
    局部变量在代码运行结束后就销毁，不占内存资源。
* 块级作用域{}
    在es6时新增块级作用域{},外面是不能使用里面的变量；
    非es6的块级作用域{}，外面是能使用里面的变量；
* 作用域链：内部函数访问外部函数的变量，采取链式查找方式来决定采用那个值。即就近原则
    ```html
    <script>
        var num = 10;
        function fn() {
            var num = 20;
            function fun(){
                console.log(num);
            }
            fun();
        }
        fn();//20
    </script>
    ```

### 九.JS的预解析
JS引擎运行JS分两步：预解析和代码执行
* 预解析：将js里的var,function提升到当前作用域的最前面
    * 变量预解析（变量提升）：将所有变量声明提升到当前作用域的最前面，不提升赋值
    函数内部的变量不会在外面提升，而是在函数内部提升；
    * 函数预解析（函数提升）:将所有函数声明提升到当前作用域的最前面，不调用函数
* 代码执行：按照代码书写顺序从上往下执行

### 十.JS的对象
* 什么是对象
    一个具体的事物。在JS中，无序的相关属性和方法的集合，所有的事物都是对象，如：字符串，数值，数组，函数等。
* 组成
    * 属性：事物的特征

    * 方法：事物的行为
* 为什么需要对象：保存对象的完整信息，结构更清晰。
* 创建对象的三种方式
    补充说明：()优先级；[]数组的字面量；{}对象的字面量
    * 字面量创建:采用键值对；逗号隔开
        ```html
        <script>
            //语法：var obj = {};
            //创建对象
            var obj = {
            uname: 'zhangsanfeng',
            age: 18,
            sex: 'female',
            say: function() {
                console.log('hi~');
            }
            };
            //使用对象
            //(1)
            console.log(obj.uname);
            //(2)
            console.log(obj['age']);
            //调用对象的方法,()是必要的
            obj.say();
        </script>
        ```
        * 案例（小狗狗）
        * 变量和属性
            * 相同点：都用来存储数据
            * 不相同点：变量是单独声明并赋值，单独存在，使用时直接写变量名；属性要在对象里，不需声明，使用时必须对象.属性
        * 方法和函数
            * 相同点：都用来实现某种功能
            * 不相同点：函数是单独声明并调用，单独存在；方法要在对象里，使用时必须 对象.方法()
   * 利用new Object创建
        ```html
        <script>
        // 利用new Object创建对象
            var obj = new Object();
            obj.uname = 'zhangsanfeng';
            obj.age = 18;
            obj.sex = 'female';
            obj.say = function(){
                console.log('hello!');
            }
            //利用等号赋值，以分号结束；调用和上述一样
            console.log(obj.sex);
            obj.say()
        </script>
        ```
        * 案例（鸣人）
    * 利用new Object创建
        ```html
            <script>
            //为什么采用构造函数：上述两种方法一次只能创建一个对象
                    //之所以叫构造函数是因为里面封装的是对象，且利用函数方法，重复相同代码
                    //即构造函数就是把对象里面一些相同的属性和方法抽象出来分封装到函数里面
                    /* function 构造函数名(){
                        this.属性 = 值;
                        this.方法 = function(){

                        }
                    }
                    new 构造函数名(); */

                    function Star(uname, age, sex){
                        this.name = uname;
                        this.age = age;
                        this.sex = sex;
                        this.sing = function(sang){
                            console.log(sang);
                        }
                    }
                    var ldh = new Star('刘德华', 18, '男');//调用函数返回对象
                    console.log(ldh.name);
                    console.log(ldh['sex']);
                    ldh.sing('忘情水');

                    var zxy = new Star('张学友', 18, '男');
                    console.log(zxy.name);
                    console.log(zxy['age']);
                    //构造函数首字母必须大写
                    //不需要return就返回结果
                    //调用时，必须使用new
                    //必须添加this,指向自身 
            </script>
        ```
* 构造函数和对象
    * 构造函数:泛指某一大类
    * 对象:特指一个具体事物
    * 对象的实例化：利用构造函数创建对象的过程
* new关键字的执行过程
    * 1.在内存中创建了一个空的对象；
    * 2.this指向刚才创建的空对象；
    * 3.执行构造函数里的代码，给空对象添加属性和方法；
    * 4.返回这个对象（即不需要return）；
* 遍历对象
    * for in
        ```html
        <script>
            var obj1 = {
                uname: 'zhangsanfeng',
                age: 18,
                sex: 'female',
                say: function() {
                    console.log('hi~');
                }
            };
            //for in遍历对象
            for(var k in obj) {
                console.log(k);//得到属性名
                console.log(obj[k]);//得到属性值
            }
        </script>
        ```

### 十一.JS的内置对象
* 什么是内置对象
* 查询指定API的使用方法
    * 查询文档：MDN；W3C
        注：参数里带中括号则该参数可有可无
        查阅方法的功能；
        查看参数的意义和类型；
        查看返回值的意义和类型；
        进行demo测试。
* Math对象
* 日期对象
* 数组对象
* 字符串对象
#### 什么是内置对象
* ECMASScript
    自定义对象
    内置对象：JS自带对象，不用关心内部如何实现，直接使用，帮组快速开发
    浏览器对象（JS独有）
#### 查询指定API的使用方法
* 查询文档：MDN；W3C
    注：参数里带中括号则该参数可有可无
    查阅方法的功能；
    查看参数的意义和类型；
    查看返回值的意义和类型；
    进行demo测试。
#### Math对象
* 非构造函数，无需new来调用
    * Math.PI
    * 封装数学对象，含最大小值
    * Math.abs
    * Math.floor向下取整，往最小的取值
    * Math.ceil向上取整，往最大的取值
    * Math.round四舍五入,负数往大的取
    * Math.random()返回随机小数，范围[0,1);方法里可无参数
    * 案例
        * 猜数字:输入1~50之间任意数，只有10次机会
        ```html
        <script>
            var num = prompt('请输入1~50的任意数字:');
            function getRandom(min, max) {
                return Math.floor(Math.random() * (max - min + 1)) + min;
            }
            var random = getRandom(1, 50);
            var temp = [];
            for (var i = 0; i < 10; i++){
                if(num == random){
                    alert('恭喜答对，程序结束');
                    break;
                } else if(num > random) {
                    alert('数字大了，继续猜');
                } else {
                    alert('数字小了，继续猜');
                }
                temp[i] = num;
                num = prompt('请输入1~50的任意数字:');
            }
            alert('10次回答已用完,下次再来');
        </script>
        ```
#### 日期对象
* Date()是一个构造函数，必须用new调用
    ```html
        <script>
            var date = new Date();
            console.log(date);
        </script>
    ```
    * date.getFullYear();
    * date.getMonth() + 1;//返回月份小1个月
    * date.getDate();
    * date.getDay();//周几 周日返回0
    * date.getHours();
    * date.getMinutes();
    * date.getSeconds();
* Date总的毫秒数（时间戳）
    ```html
    <script>
        var date = new Date();
        //(1)
        console.log(date.valueOf());
        //(2)
        console.log(date.getTime());
        //(3)
        var date1 = +new Date();
        console.log(date1);
        //(4)
        console.log(Date.now());//H5新增 获得总的毫秒数
    </script>
    ```
* 案例
    * 倒计时效果
        ```html
        <script>
            function cuntDown(time){
            var nowTime = +new Date();
            var inputTime = + new Date(time);
            var times = (inputTime - nowTime) / 1000;//1秒=1000毫秒，获得总的秒数times
            var d = parseInt(times / 60 / 60 / 24);//parseInt()用于将字符串解析为整数。
            d = d < '10' ? '0' + d : d ;
            var h = parseInt(times / 60 / 60 % 24);
            h = h < '10' ? '0' + h : h ;
            var m = parseInt(times / 60 % 60);
            m = m < '10' ? '0' + m : m ;
            var s = parseInt(times % 60);
            s = s < '10' ? '0' + s : s ;

            return '倒计时' + d + '天' + h + '时' + m + '分' + s + '秒'
            }
            console.log(cuntDown('2024-2-15 18:00:00'));
        </script>
        ```       
#### 数组对象
* 创建方式
    * （1）利用new
    ```html
    <script>
        var arr = new Array();

        var arr1 = new Array(2);//2表示数组长度，里面有2个空的数组元素
        var arr2 = new Array(2, 3);//等价于[2,3],里面有2个数组元素，想放元素就得写2个以上的数
    </script>
    ```
    * （2）数组字面量
    ```html
    <script>
        var arr = [1, 2, 3, 4]
    </script>
    ```
* 检测是否为数组
    * instanceof
    * Array.isArray()优先于instanceof，H5新增，ie9以上支持
        ```html
        <script>
            var arr1 = [];
            var obj = {};
            console.log(arr1 instanceof Array);
            console.log(obj instanceof Array);

            console.log(Array.isArray(arr1));
            console.log(Array.isArray(obj));
        </script>
        ```
* 添加/删除数组元素
    * push():数组末尾添加1个及以上的元素,有参数
    * unshift():数组开头添加1个及以上的元素,有参数
    * pop():删除数组的最后一个元素,没有参数
    * shift():删除数组的第一个元素,没有参数
    * 案例
        * 筛选数组
            ```html
            <script>
                var arr = [1500, 1200, 2000, 2100, 1800];
                var Arr = [];
                for(var i = 0; i < arr.length; i++){
                    if (arr[i] < 2000){
                        Arr.push(arr[i]);    
                    }
                }
                console.log(Arr);
            </script>
            ```
        * 翻转数组reverse()
            ```html
            <script>
                var arr = [1500, 1200, 2000, 2100, 1800];
                arr.reverse();//重点
                console.log(arr);
            </script>
            ```
        * 数组的冒泡排序sort()
            ```html
            <script>
                var arr = [1500, 1200, 2000, 2100, 1800];
                arr.sort();//重点
                console.log(arr);

                var arr1 = [13, 4, 77, 1, 7];
                arr1.sort();
                console.log(arr1);// [1, 13, 4, 7, 77]结果并非期望那样

                arr1.sort(function(a, b) {
                    return a - b;//升序排列；若b -a则为降序排列
                });
                console.log(arr1);
            </script>
            ```
        * 返回数组元素的索引号indexOf()
            * 只返回第一个满足条件的索引号
            * 若在数组里未找到对应元素则返回-1；
            * indexOf('red')从前往后
            * lastIndexOf('red')从后往前
                ```html
                    <script>
                        var arr = ['red','green','pink','white','red','black'];
                        console.log(arr.indexOf('red'));  
                    </script>
                ```
            * 案例：数组去重
                ```html
                    <script>
                        function unique(arr){
                            var elements = [];
                            for (var i = 0;  i< arr.length; i++){
                                if (elements.indexOf(arr[i]) === -1){
                                    elements.push(arr[i]);
                                }
                            }
                            return elements;
                        }
                        var alone = unique(['c','a','z','a','x','a','x','c','b']);
                        console.log(alone); 
                    </script>
                ```
        * 数组转换为字符串
            * toString()
                ```html
                    <script>
                        var arr = [1,2,3];
                        console.log(arr.toString());
                    </script>
                ```
            * join('分隔符'),返回字符串
                ```html
                    <script>
                        var arr1 = ['red','green','pink'];
                        console.log(arr1.join());
                        console.log(arr1.join('-'));
                    </script>
                ```
            * concat():连接多个数组返回新数组，不影响原数组
                ```html
                    <script>
                        var arr1 = ['c','a','z'];
                        var arr2 = [1,2,3];
                        var array3 = arr1.concat(arr2);
                        console.log(array3);
                    </script>
                ```
            * slice():返回截取的新数组，不影响原数组
                ```html
                    <script>
                        var arr = ['red','green','pink','white','black'];
                        console.log(arr.slice(2,-1)); 
                    </script>
                ```
            * splice():返回删除的元素组成的新数组，会影响原数组
                ```html
                    <script>
                        var months = ['Jan', 'March', 'April', 'June'];
                        months.splice(1, 0, 'Feb');//第一个数字表位置，第二个数字表替换的元素数
                        console.log(months);
                        //console.log(months.splice(1, 0, 'Feb'));//这种写法输出无效
                        months.splice(4, 1, 'Maybe');
                        console.log(months);
                    </script>
                ```             
#### 字符串对象
* 简单数据类型是不存在属性和方法
* 对象和复杂数据类型才有属性和方法
* 基本包装类型就是将简单数据类型包装成复杂数据类型
    ```html
        <script>
            var str = 'andy';
            console.log(str.length);
            //上述实际变化是---------------
            var temp = new String('andy');
            str = temp;
            temp = null;
            //字符串的不可变，看上去好像是字符串的内容改变了，实际上是在内存中重新开辟空间存储并指向新空间
            var str = 'andy';
            console.log(str);
            str = 'red';
            console.log(str);   
        </script>
    ```
* 根据字符串返回位置,可以指定起始位置indexOf()
    ```html
    <script>
        var str = '今天是星期天';
                console.log(str.indexOf('天'));//1
                console.log(str.indexOf('天',2));//5 
    </script>
    ```
* 返回字符串中某个元素出现的位置及次数indexOf()
    ```html
    <script>
    var text = 'abcoefoxyozzopp';
                var start = text.indexOf('o');
                var num = 0;
                while(start !== -1){
                    console.log(start);
                    num++;
                    start = text.indexOf('o',start + 1);
                }
                console.log(num);
    </script>
    ```
* charAt():根据位置返回字符
    ```html
        <script>
            var str ='word';
            console.log(str.charAt(2));   
        </script>
    ```
* charCodeAt():返回相应索引号的字符ASCII码
    ```html
        <script>
            var str ='word';
            console.log(str.charCodeAt(0));   
        </script>
    ```
* str[],H5新增
    ```html
        <script>
            var str ='word';
            console.log(str[0]);
        </script>
    ```
* 案例
    * 统计出现最多的字符和次数
        ```html
            <script>
                var text = 'abcoefoxyozzopp';
                var obj = {};
                for(var i = 0; i < text.length; i++){
                    var element = text.charAt(i);
                    if(obj[element]){
                        obj[element]++;
                    }else {
                        obj[element] = 1;
                    }
                }
                console.log(obj);
                var max = 0;
                for(var key in obj){
                    if(obj[key] > max){
                        max = obj[key];
                        ch = key;
                    }
                }
                console.log('出现最多的字符'+ch+'出现次数'+max); 
            </script>
        ```
* 字符串操作方法
    * concat():连接
    * substr(位置,截取字数):截取
    * replace:替换，只能替换第一个字符串
    * split('分隔符'):字符转换为数组;join('分隔符'):数组转换为字符串
    * 综合案例
        ```html
            <script>
                var str = 'sky';
                var text = str.concat('scraper');
                console.log(text);
        
                var result = text.substr(2,2);
                console.log(result);//ys
        
                var rep = result.replace('s', 'y');
                console.log(rep);//yy
                var text = rep.concat('scraper');
                console.log(text);//yyscraper
              
                while(text.indexOf('r') !== -1){
                    text = text.replace('r', '$');
                }
                console.log(text);
               
                var arr = text.split('$');
                console.log(arr);
            </script>
        ```
    * toUpperCase()转换为大写
    * toLowerCase()转换为小写

### 十二.JS简单数据类型和复杂数字据类型
* 数据类型
    * 简单数据类型
    * 复杂数字据类型
* 堆和栈
* 内存分配
* 传参注意事项
#### 数据类型
* 简单数据类型
    简单数据类型（基本数据类型或值类型）：在存储时变量中存储的是值本身，故又叫值类型
    常用的简单数据类型：string, number, boolean, undefined, null
* 复杂数字据类型
    复杂数字据类型（引用数据类型）:变量中存储的仅仅是地址，故又叫引用数据类型。通过new来创建的对象（系统对象，自定义对象）
    常用的复杂数字据类型：Object,Array,Date
#### 堆和栈
    栈(操作系统)：由操作系统自动释放；操作方式类似于数据结构中的栈；简单数据类型存放到栈里
    堆(操作系统)：由程序员分配释放，若没释放就由垃圾回收机制回收；复杂数据类型存放到堆里
    注：JS中没有堆栈的概念，上述值为便于理解代码的执行方式
#### 内存分配
    简单数据类型：直接在栈里找数据
    复杂数据类型：先到栈里找地址，再到堆里找数据
#### 传参注意事项
    简单数据类型：在栈里是按照值来进行存储的。声明变量便会在栈中开辟空间，放入值，变量指向值。
    简单类型传参不会相互影响
    复杂数据类型：会相互影响

### 十三.Web APIs
* JS基础和Web APIs
    * JS基础:基本语法
    （）==> JS基础
    * Web APIs:JS的应用
    （）==> Web APIs 
* API()
    给程序员提供的一种（），使其轻松实现想要完成的功能，（）即可，无需纠结（）实现。
* Web API   
    本质上也是一个（）。由（）提供的一套（）和（）的API()。  
    主要针对浏览器提供的（），对浏览器做（）效果
    一般都有输入和输出（），很多都是方法（）
    可结合（）方法的思路学习
* DOM
    * DOM简介
        DOM（）：处理可扩展标记语言()的()接口，即处理()的接口。
        用这些接口可以改变网页的()，()和()。
        * DOM树：包含（）（）（）。
    * 获取元素：有（）种方法，分别是哪些？
    * 事件基础
        * 事件三要素
            事件源指（）；事件类型指（）;事件处理程序指（）


    * 操作元素
    * 案例
    * 节点操作
#### Web APIs和JS基础
* JS基础:基本语法
    ECMAScript ==> JS基础
* Web APIs:JS的应用
    DOM 和 BOM ==> Web APIs 
#### API(应用程序编程接口)
    给程序员提供的一种工具（接口），使其轻松实现想要完成的功能，会用即可，无需纠结内部如何实现。
#### Web API
  本质上也是一个接口。由/浏览器/提供的一套/操作浏览器功能/和/页面元素/的API(BOM和DOM)。  
  主要针对浏览器提供的接口，主要针对浏览器做交互效果
  一般都有输入和输出（函数的传参和返回值），很多都是方法（函数）
  可结合内置对象方法的思路学习
#### DOM
* DOM简介
    DOM（文档对象模型）：处理可扩展标记语言(HTML,XML)的标准编程接口，即处理文档/页面的接口。
    用这些接口可以改变网页的内容，结构和样式。
    * DOM树：
        * 文档：一个页面就是一个文档；
        * 元素：页面中的所有标签；
        * 节点：所有内容都是节点(标签，属性，文本，注释等).
        注：DOM把以上都看做对象。
* 获取元素
    * 根据ID获取元素
        ```html
            <script>
            // 根据ID获取元素
                var timer = document.getElementById('time');//返回对象
                console.log(timer);
                console.log(typeof timer);
                // console.dir() 打印我们返回的元素对象，更好查看里面的属性和方法
                console.dir(timer)
            </script>
        ```
    * 根据标签名获取
        ```html
            <script>
                //根据标签名获取
                //返回的是 所获取元素对象的集合 以伪数组的形式存储
                //若页面中没有元素，则返回空的伪数组
                var lis = document.getElementsByTagName('li');
                console.log(lis);
                console.log(lis[0]);
                //依次打印对象，用遍历
                for (var i = 0; i < lis.length; i++) {
                    console.log(lis[i]);
                    
                }
            </script>
        ```
        * 获取某个元素内部所有指定标签名的子元素
            element（父元素）.getElementsByTagName('标签名');
            ```html
                <script>
                    //伪数组不能作为父元素
                    var ol = document.getElementsByTagName('ol');
                    console.log(ol[0].getElementsByTagName('li'));
                    // console.log(ol.getElementsByTagName('li'));//伪数组不能作为父元素
                    var ol = document.getElementById('ol');
                    console.log(ol.getElementsByTagName('li'));
                </script>
            ```
    * 根据类名获取,H5新增，ie9以上使用
        ```html
            <script>
                var boxs = document.getElementsByClassName('box');
                console.log(boxs);
            </script>
        ```
    * 不管选择器类型
        * querySelector() 获取第一个元素对象
            ```html
                <script>
                    var firstBox = document.querySelector('.box');
                    console.log(firstBox);

                    var nav = document.querySelector('#nav');
                    console.log(nav);

                    var li = document.querySelector('li');
                    console.log(li);
                </script>
            ```
        * querySelectorAll() 获取所有元素对象集合
            ```html
                <script>
                    var allBox = document.querySelectorAll('.box');
                    console.log(allBox);
                </script>
            ```
    * 获取特殊元素
        * 获取body (document.body)
            ```html
                <script>
                    console.log(document.body);
                    console.dir(document.body);
                </script>
            ``
        * 获取html (document.documentElement)
            ```html
                <script>
                    console.log(document.documentElement);
                </script>
            ``
* 事件基础
    * 事件三要素
        * 事件源（事件被触发的对象）；
            谁被触发，点击？
        * 事件类型（如何触发 onclick）;
            通过什么触发?
        * 事件处理程序（通过一个函数赋值的方式 完成）
            要做啥
        * 案例
            ```html
                <script>
                // 执行事件步骤
                    //1.获取事件源
                    var click = document.querySelector('div');
                    //2.绑定事件 注册事件
                    //div.onclick
                    //3.添加事件处理程序
                    div.onclick = function() {
                        console.log('on clicked');
                    }
                </script>
            ```
        * 常见事件类型
            onclick:鼠标左击触发
            onmouseover:鼠标经过
            onmouseout:鼠标离开
            onfocus:获得鼠标焦点
            onblur:失去鼠标焦点
            onmousemove:鼠标移动
            onmouseup:鼠标弹起触发
            onmousedown:鼠标按下触发
* 操作元素
    * 修改元素内容
        * element.innerText
            不识别HTML标签，非标准；去除换行和空格
            ```html
                <script>
                // 执行事件步骤
                    //1.获取元素
                    var div = document.querySelector('div');
                    var btn = document.querySelector('button');
                    //2.绑定事件 注册事件
                    //btn.onclick
                    btn.onclick = function() {
                    //3.1添加事件处理程序
                        div.innerText = '2020-01-01';
                    }

                    //3.2不添加事件处理程序
                    div.innerText = '2020-01-01';
                </script>
            ```
        * element.innerHTML
            识别HTML标签，w3c推荐；保留换行和空格
            ```html
                <script>
                // 执行事件步骤
                    //1.获取元素
                    var div = document.querySelector('div');
                    //3.2不添加事件处理程序
                    div.innerText = '<strong>today is<\strong>:2020-01-01';
                    div.innerHTML = '<strong>today is<\strong>:2020-01-01';
                </script>
            ```
    * 修改元素属性
        ```html
            <button id="man">man</button>
            <button id="woman">woman</button>
            <img scr="man.jpg" alt="" title="man">
            <script>
                var man = document.getElementById('man');
                var woman = document.getElementById('woman');
                var img = document.querySelector();

                man.onclick = function(){
                    img.src = 'woman.jpg';
                    img.title = 'woman';
                }
                woman.onclick = function(){
                    img.src = 'man.jpg';
                    img.title = 'man';
                }
            </script>
        ```
        * 分时显示不同图片与问候语
            ```html
                <body>
                    <img src="#" alt="">
                    <div>good morning</div>
                    <script>
                    // 判断时间,用到系统的内置时间
                    // 设置不同图片
                    // 根据时间修改不同图片
                    // 需要显示不同问候语，修改元素内容
                    var img = document.querySelector('img');
                    var div = document.querySelector('div');
                    var date = new Date();
                    var h = date.getHours();
                    if(h < 12) {
                        img.src = 'morning.jpg';
                        div.innerHTML = 'good morning';
                    } else if (h < 18) {
                        img.src = 'afternoon.jpg';
                        div.innerHTML = 'good afternoon';
                    } else {
                        img.src = 'evening.jpg';
                        div.innerHTML = 'good evening';
                    }
                    
                    </script>
                </body>
            ```       
    * 表单属性设置
        ```html
            <button>button</button>
            <input type="text" value="input please">
            <script>
                var btn = document.querySelector('button');
                var input = document.querySelector('input');

                btn.onclick = function(){
                    //innerHTML用于div等普通盒子
                    //表单内值通过value改变
                    input.value = 'inputted';
                    //点击后按钮被禁用
                    this.disabled = true;//btn.disabled = true
                }
                
            </script>
        ```
        * 查看密码明文案例
            ```html
                <input type="password">
                <button>change</button>
                <script>
                    var ps = document.querySelector('input');
                    var btn = document.querySelector('button');
                    var flag = 0;
                    btn.onclick = function() {
                        
                        if(flag == 0){
                            ps.type = 'text'; 
                            return flag = 1;
                        } else {
                            ps.type = 'password';
                            return flag = 0;
                        }
                    }
                </script>
            ```
    * 样式属性操作
        * element.style:行内样式操作
            JS的样式权重高于css；JS的样式采用驼峰命名法
            ```html
                <style>
                    div {
                        background-color: rgb(143, 220, 220);
                        width: 200px;
                        height: 200px;
                    }
                </style>
                <body>
                    <div></div>
                </body>
                <script>
                    var div = document.querySelector('div');
                    div.onclick = function() {
                        div.style.backgroundColor = 'red';
                        div.style.width = '300px';
                        div.style.height = '300px';
                    }
                </script>
            ```
            display:none 显示
            display:block 隐藏
            * 案例-关闭二维码
            * 案例-循环精灵图???
            * 案例-显示隐藏文本框内容
        * element.className:类名样式操作,更改当前元素的类名
            * 案例-密码提示错误信息
                分析：
                    首先判断表单失去焦点onblur；
                    若输入正确则提示正确信息的绿色小图标变化；
                    若输入不是6到16位，则提示错误信息颜色为红色，小图标变化
    * 元素属性值操作
        * element.属性:元素本身内置
        * element.属性 = '值':设置元素属性值
            ```html
            <div id="memo"></div>
            <script>
                var div = document.querySelector('div');
                //element.属性:元素本身内置,获取属性值
                console.log(div.id);
                // element.属性 = '值':设置元素属性值
                div.id = 'test';
            </script>
            ```
        * element.getAttribute('属性')：获得自定义属性
        * element.setAttribute('属性','值')：设置自定义属性
        * element.removeAttribute('属性')：移除属性
            ```html
            <div id="memo" index="1"></div>
            <script>
                var div = document.querySelector('div');
                //element.getAttribute('属性')：获得自定义属性
                console.log(div.getAttribute('id'));
                //element.setAttribute('属性','值')：设置自定义属性
                console.log(div.setAttribute('id','test'));
                //element.removeAttribute('属性')：移除属性
                div.removeAttribute('index');
            </script>
            ```
        * H5自定义属性
            * 目的：保存并使用数据，某些数据可以保存到页面而不保存到数据库中。
            * 判断自定义属性：以data-开头作为属性名并赋值
            * dataset：存放了所有以data开头的自定义属性，h5新增，ie11开始支持。
            ```html
            <div getTime="20" data-index="2" data-list-name="Tomboy">qw</div>
            <script>
                var div = document.querySelector('div');
                console.log(div.getAttribute('getTime'));
                div.setAttribute('data-time', 15);
                console.log(div.getAttribute('data-index'));
                console.log(div.getTime);//自定义属性的值的获取不能采用元素内置的方法
                //h5新增，ie11开始支持。dataset是一个存放了所有以data开头的自定义属性
                console.log(div.dataset);
                console.log(div.dataset.index);
                console.log(div.dataset['index']);
                //若自定义属性名里有多个连接的单词，获取是采用驼峰命名法
                console.log(div.dataset['listName']);//Tomboy
            </script>
            ```
* 案例
    * 排他思想
    * 背景换肤
    * 表格隔行换色
    * 表单全选与取消
    * tab栏页面切换(重要)
* 节点操作
    * 为什么学节点操作
        主要目的是获取元素
        获取元素常用两种方法：
        * 利用DOM提供的方法获取（缺点：繁琐，逻辑性不强）
        * 利用节点层级关系获取元素
            利用父子兄关系获取元素
            逻辑性强，兼容性稍差
    * 概述：页面中所有内容都是节点，所有节点都可以通过JS来访问，所有节点可被修改，创建或删除
    标签 -- 元素节点（nodeType=1）
    文字 -- 文本节点（nodeType=3）
    属性 -- 属性节点（nodeType=2）
    空格与换行也是节点，统称为文本节点
    节点的三个基本属性：节点类型（nodeType），节点名称（nodeName），节点值（nodeValue）
    注：实际开发中，节点操作主要是元素节点
    * 节点层级
        常见父子兄层级
        * 父节点:parentNode
            ```html
            <div id="QR_code">
                <img src="resorces\img\QR_code.png" alt="">
                <i id="close-btn">X</i>
            </div>
            <script>
            var close_btn = document.getElementById("close-btn");
            // 父节点parentNode,得到的是离元素最近的父级，若找不到则返回为空
            console.log(close_btn.parentNode);
            </script>
            ```
        * 子节点
            ```html
            <body>
                <ul>
                    <li>Do you want a cup of coffee or milk?</li>
                    <li>Do you want a cup of coffee or milk?</li>
                    <li>Do you want a cup of coffee or milk?</li>
                    <li>Do you want a cup of coffee or milk?</li>
                </ul>
                <ol id="ol">
                    <li>Do you want a cup of coffee or milk?</li>
                    <li>Do you want a cup of coffee or milk?</li>
                    <li>Do you want a cup of coffee or milk?</li>
                    <li>Do you want a cup of coffee or milk?</li>
                </ol>
                <script>
                    //子节点
                    //(1)子节点childNodes得到所有节点，包含换行等,一般不提倡用
                    var ul = document.querySelector('ul');
                    console.log(ul.childNodes);//获得9个节点

                    //(2)parentNode.children获取所有的子元素节点
                    console.log(ul.children);
                    //子节点属性
                    //firstChild获取第一个子节点，不管节点类型
                    //firstElementChild获取第一个元素子节点
                    console.log(ul.firstChild);
                    console.log(ul.lastChild);
                    console.log(ul.firstElementChild);//ie9以上支持
                    console.log(ul.lastElementChild);//ie9以上支持
                    //(3)实际开发常用，既无兼容性问题又返回第一个子元素
                    console.log(ul.children[0]);
                    console.log(ul.children[3]);
                    console.log(ul.children[ul.children.length - 1]);
                </script>
            </body>
            ```
        * 兄弟节点 
            nextSibling:下一个兄弟节点
            previousSibling:上一个兄弟节点
            下列h5新增，ie9以上支持
            nextElementSibling:下一个兄弟元素节点
            previousElementSibling:上一个兄弟元素节点
            解决兼容性问题见（兄弟节点.html）
    * 动态创建节点（动态创建节点.html）
        * createElement():创建节点
        * node.appendChild(child):添加节点
        * node.insertBefore(child,指定插入哪个元素的前面):将元素插入指定元素之前
        * 点击发布案例.html
    * 删除节点 (点击发布案例.html)
        node.removeChild
        * 每个评论都添加删除功能(点击发布案例.html)
            javascriptvoid(0):阻止链接跳转 === javascript:;
    * 复制节点（克隆节点）
        node.cloneNode():括号里为空或者false则为浅拷贝，只复制节点本身，不含内容；为true就都拷贝
    * 案例-动态表格生成.html
    * 三种创建元素方式区别(三种创建元素方式区别.html)
        * document.write()
        * innerHTML和createElement
            不同的浏览器，innerHTM（结构稍微复炸）L在不拼接字符串，采取数组的形式的情况下效率比createElement（结构清晰）高


### 十四.事件高级
* 元素注册事件的两种方式(注册事件.html)
    * 传统方式
        on开头的事件；
        注册事件具有唯一性，同一个元素同一个事件只有一个监听器
    * 利用方法监听注册方式
        addEventListener()在IE9之前不支持，可使用attachEvent()代替；
        同一个元素同一个事件可以注册多个监听器；
        按注册顺序依次执行.
        注：attachEvent()非标准，尽量不在生产环境中使用
    * 处理兼容性的原则：
        先照顾大多数浏览器，再处理特殊浏览器    
* 删除事件的两种方式(删除事件.html)
    * 传统方式
        element.onclick = null;
    * 利用方法监听注册方式
        element.removeEventListener('click', fn);
        * attachEvent()
            element.detachEvent('onclick', fn1);

* DOM事件流的三个阶段（DOM事件流.html）
    * 事件流：从页面中[接收事件的顺序]。
        事件发生时会在元素节点之间[按照特定的顺序传播]，这个[传播过程]即DOM事件流。
        * 捕获阶段：从顶层向下一层一层寻找的过程，每层都会接收事件，若有处理操作就执行，没有就向下继续捕获。
        * 当前目标阶段
        * 冒泡阶段：从底层向上依次传播事件。
    * 注意：
        JS只能执行捕获或者冒泡其中一个阶段；
        onclick和attachEvent只能得到冒泡阶段。
        addEventListenter(type, listener[, useCapturel])第三个参数若是true，表示在事件捕获阶段调用事件处理程序；
        若是false，表示在事件冒泡阶段调用处理程序。
        冒泡使用更多。
    * 没有冒泡的事件
        * onblur
        * onfocus
        * onmouseenter
        * onmouseleave
* 事件对象（事件对象.html）
    事件发生后，与事件相关的一系列信息数据的集合到放在对象event中,这个对象就叫事件对象，它含有很多属性和方法。
    * 事件对象特点
        事件对象event是写到侦听函数function()的括号中的形参,不需要再传递参数；
        事件对象只有有了事件才会存在，是系统自动创建，不需要我们传递参数，可以对事件对象event进行命名；
        事件对象是事件一系列相关数据的集合，如鼠标单击事件就包含鼠标相关信息，如坐标等；
        事件对象也有兼容性问题，ie678是通过window.event得到事件对象
    * 兼容性问题
        常通过e || window.event来解决
    * 事件对象常见的属性和方法（事件对象属性方法.html）
        * e.target:点击对象返回(标准)
        this/currentTarget(有兼容性问题，不常用非标准，了解即可)：绑定对象返回
        * e.type()返回事件类型
        * 阻止事件默认行为   
            e.preventDefault() //这是方法
            e.returnValue//这是属性
        * 阻止冒泡事件的两种方式（DOM事件流.html）
            * e.stopPropagation();标准 阻止冒泡
            * e.cancelBubble = true;//不起作用，只适用低版本浏览器
    * 事件委托（事件委托.html）
        事件委托又称事件代理,在JQuery中叫事件委派 
        在同类型的事件中进行一样的操作时（如警示框弹出），但当有成百上千个同类型元素都需要同样操作时，就需要在每个元素中都添加警示框，这会导致程序繁琐，效率低下，因此使用事件委托，由父元素代理对每个子元素的点击，使用e.target再返回被操作的元素本身。  
* 利用事件对象完成跟随鼠标案例
* 封装阻止冒泡的兼容性函数
* 事件委托的原理
* 常用的鼠标和键盘事件(鼠标和键盘事件.html)
    * contextmenu :禁用右键菜单
    * selectstart ：禁止选中文字
    * 鼠标事件对象
        e.clientX/clientY ：相对于浏览器窗口的位置
        e.pageX/pageY ：相对于文档页面的位置,IE9以上支持
        e.screenX/screenY ：相对于电脑屏幕的位置
        * 案例
            图标跟随鼠标.html
    * 键盘事件对象(键盘事件对象.html)
        * onkeyup:按键松开时触发
        * onkeydown：按键按下时触发
        * onkeypress：按键按下触发，功能键除外
        注：执行顺序onkeydown > onkeypress > onkeyup,传统用法加on，addEventListener不用加
        只要有事件就有事件对象
        keyup,keydown不区分字母大小写，按下a或A都是65.
        keypress区分字母大小写
        keyCode得到ASCII码值，可以判断用户按下哪个键。



