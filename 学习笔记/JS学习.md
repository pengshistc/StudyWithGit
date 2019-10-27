## ***JS学习***
---
### 1. JS 的声明引入和变量声明和变量类型

* **JS 的声明学习**
    1. 在 **head标签**中使用 **script标签** 进行 **js代码域**的声明
        * **代码展示**
        ```
        <script type="text/javascript">
            alert("...") 
        </script>
        ```
        * **特点**（js的代码只会作用于当前网页）
        
    2. 在 **head标签**中使用 **script标签** 引入外部js文件
        * **代码展示**
        ```
        <script src="..." type="text/javascript" charset="utf-8"></script>
        ```
        * html5代码中可以去掉 **type="text/javascript"**
    
    3. js代码与页面代码的相对位置控制了展示出来的顺序

    4. js中变量声明只有 var 关键字

    5. js的变量名严格区分大小写

    6. js中字符串可以使用单引号和双引号，需要成对出现

    7. js可以声明同名变量，后面会覆盖前面

    8. 数据类型
        * 数据类型判断关键字：**typeof**
        * **number**（整型，浮点型都是number类型）
        * **string**（无字符和字符串区分，单引号和双引号无区别）
        * **boolean**
        * **object**
        * **null**
        * **Undefined**(变量声明不赋值/不存在)
        
### 2. JS 的变量
    
* **JS 的变量声明**
    1. 变量的作用 **：** 存储数据，方便程序进行操作

* **JS 变量的特点**
    1. 变量声明关键字 **：** **var**
    2. JS 中的代码可以不使用分号结尾
    3. JS 中的变量允许出现同名变量，但是后面的会将前面的覆盖
    4. 声明未赋值，默认值是undefined

* **JS 的数据类型**
    1. 使用 **typeof** 判断变量的数据类型
        * number：数值类型
        * string：字符类型（在js中字符可以使用单引号，也可以使用双引号）
        * boolean：布尔类型
        * object：对象类型

* **JS 的变量强制转换**
    1. 使用 **Number()函数** ，将其他数据类型转换为数值类型，转换失败返回 NaN ,**NaN**为数值类型
    2. 使用 **Boolean()函数** ，将其他数据类型转换为布尔类型，有值返回true，无值或者值为0返回false

* **特殊的值**
    1. **null** (数据类型为：**object**)
    2. **undefined**(数据类型为：**undefined**)
    3. **NaN**(数据类型为：**number**)

### 3. JS 的运算符

* **算数运算符**
    1. 加法（+）
    2. 减法（-）
    3. 乘法（*）
    4. 除法（/）
    5. 余数（%）
    * 运算类型：
        1. number类型和number类型
        2. number类型和boolean类型（true = 1 ； false = 0）
        3. number类型和string类型（-，*，/，%）
        4. string类型和string类型的数字（-，*，/，%）
        5. string类型和boolean类型（-，*，/，%）
        * 在算术运算中如果两边的数据类型不是number的话，会使用Number()强制转换后再进行运算
        * **注意：** 在字符串中“+”代表的是字符串的连接符，不参与运算

* **逻辑运算符**
    1. !
    2. & （按位异或）
    3. && （逻辑判断）
    4. |
    5. ||

* **关系运算符**（返回值为true或者false）
    1. !=
    2. >=
    3. <=
    4. >
    5. <

* **自增运算符**
    1. ++
    2. --
    3. +=（位运算效率更高？）
    4. -=

### 4. JS 的 == 和 === 运算符

* **等值运算符 ==**
    * **例子：**
        * **代码：**
        var a=1;
        var a1="1";
        var a2=true;
        var a3="true";
        var a4="a";
        var a5="a";
        * **结果：**
        a==a1;//true
        a==a2;//true
        a==a3;//false
        a1==a2;//true
        a1==a3;//false
        a2==a3;//false

    * 类型一致则直接比较；
    类型不一致，则先使用Number()进行强转后再进行比较；

* **等同运算符**
    * 先判断类型，类型一致再比较内容，内容相同才返回true，否则返回false

* **注意：**
    1. null==undefined;//true
    2. 对象类型和基础类型相比较使用toString()或者valueOf()比较



### 5. JS 的逻辑结构

* **1.if结构**
    * 单分支结构
        * if(判断条件){执行体}
    * 双分支结构
        * if(判断条件){执行体}else{执行体}
    * 多分支结构
        * if(判断条件){执行体}else if(判断条件){执行体}...

* **switch选择结构**
    * 判断的变量可以是number类型，也可以是string类型，但是不要混用
    * === 等值判断

* **循环结构**
    * for循环
    * while循环
    * do while循环


### 6. JS 的数组(1)

* **声明方式**
    1. var arr = new Array();//声明一个空数组
    2. var arr = new Array(5);//声明一个长度为5的数组
    3. var arr = []; //声明一个空数组
    * **注意：** JS中的数组声明不用指定长度，JS的数组长度是不固定的，会随着元素数量的改变而改变。

* **数组的赋值和取值**
    1. 声明数组
    2. JS 的数组可以存储任意类型的数据
    3. 不存在返回undefined

* **数组的length属性**
    1. 获取数组的长度
    2. 改变数组的长度

* **数组的遍历**
    1. for 循环遍历
    2. for in遍历
    for(var i in arr){...}

### 7. JS 计算器小练习

### 8. JS 的数组(2)

* **1.数组的合并（concat）**

* **2.数组指定间隔符转换字符串（join）**

* **3.数组移除最后一个元素并返回最后一个元素的值（pop）**

* **4.数组的追加，返回新的长度值（push）** 

* **5.数组的反转（reverse）**

* **6.移除数组的第一个元素并返回该元素值（shift）**

* **7.将指定元素插入到数组的开始位置并返回该数组的长度（unshift）**

* **8.数组的排序（sort）**

* **9.从一个数组中移除一个或者多个元素（splice），返回移除的元素**
    * 起始位置，删除的个数，插入的元素

* **10.（toString）**

* **11.（valueOf）**

### 9. JS 的函数学习

* **1.声明函数**
    * **方式一**
    function 函数名(形参1,形参2,...){执行体1}
    * **方式二**
    var 函数名 = new Function("形参一","形参二",...,"函数执行体")
    * **方式三**
    var 变量名 = function(形参1，形参2,...){执行体}

* **函数的参数**
    * 函数的形参赋值可以不完全

* **函数的返回值**

* **函数的执行符号**

* **函数作为实参传递**

### 10. JS 自定义类学习

* **1.类的声明**
    * 代码
    function 类名(形参1,形参2,...){
        this.属性名1 = 形参1;
        this.属性名2 = 形参2;
        ...

        this.test = function(){执行体}
    }

* **2.类的使用**
    * var p1 = new Person("张三",32);
    alert(p1.name);


* **3.类的继承**
    * prototype关键字（实现不同对象之前的数据共享）
        * 作用1：实现某个类的所有子对象的方法区对象的共享，节省内存

### 11. JS 的自定义对象（new 个对象）

* **对象的作用：** 用来存储整体数据

### 12. JS的常用方法和对象

* **String对象**
    * 大写（toUpperCase()）
    * 小写（toLowerCase()）
    * 字符串截取
        * substr(a,b)   //a位置开始长度b
        * substring(a,b)    //a位置到b位置，含头不含尾
    * 查找字符位置
        * indexOf   //返回指定字符第一次出现的位置
        * lastIndexOf   //返回指定字符最后一次出现的位置

* **Date对象**(获取的是客户端的时间)
    * 返回从1900年至今的年数（getYear()）
    * 返回当前的年份（getFullYear()）
    * 获取当前的月份数（getMonth()+1）
    * 返回当前的日期（getDate()）
    * 返回星期数（getDay()）
    * 返回小时数（getHours()）
    * 返回当前分钟数（getMinutes()）
    * 返回当前秒数（getSeconds()）

* **Math对象**
    * random()
    * round()（四舍五入）
    * ceil()（向上取整）
    * floor()（向下取整）

* **Global对象**
    * eval()（字符串运算）
    * isNaN()
    * parseInt()
    * parseFloat()

### 13. JS 事件机制学习（一）

* **解释：** 当我们的行为动作满足一定的条件之后，会触发某类事务的执行
* **一个HTML元素可以添加多个事件**
* **内容：**
    * 单双击事件
        * 单击事件（onclick()）
        * 双击事件（ondblclick()）
    * 鼠标事件
        * 鼠标悬停（onmouseover()）
        * 鼠标移动（onmousemove()）
        * 鼠标移出（onmouseout()）
    * 键盘事件
        * 键盘弹起（onkeyup()）
        * 键盘按下（onkeydown()）
    * 焦点事件
        * 获取焦点（onfocus()）
        * 失去焦点（onblur()）
    * 页面加载事件
        * onload()  //页面加载成功后再加载

### 14. JS 事件机制学习（二）

* **1.给合适的HTML标签添加合适的事件**
    * onchange-----select下拉框
    * onload-----body标签
    * 单双击-----用户会进行点击动作的HTML元素

* **2.给HTML元素添加多个事件时，注意事件之间的冲突**
    * 单击和双击事件

* **3.事件的阻断**
    * 当事件所监听的函数将返回值返回给函数时：
        * false：会阻断当前事件所在的HTML标签的功能
        * true：继续执行当前事件所在的HTML标签的功能

* **4.超链接调用js函数**
    * `<a href="javascript:函数名()">...</a>`

### 15. JS 的 window 对象学习

* **window对象使用学习**
    * window对象不用new，直接使用即可
    * 框体方法
        * alert：警告框
        * confirm：确认框（提示用户选择一项操作 **确定/取消** ，点击确定返回**true**，点击取消返回**false**）
        * prompt:提示框（提示用户输入 **?** 点击确定返回输入值，默认返回空字符串；点击取消，返回null）
    * 定时和间隔执行方法
        * setTimeout:指定的时间后执行指定的函数
            * 参数一：函数对象
            * 参数二：时间，单位毫秒
        * setInterval：每间隔指定的时间执行指定的函数
            * 参数一：函数对象
            * 参数二：时间，单位毫秒
        * clearTimeout:停止指定的定时器
        * clearInterval: 停止指定的定时器
    * 子窗口方法
        * window.open('URL','打开方式','配置 ')
        * window.close()    //只能关闭window.open打开的页面
    * 子页面调用父页面的函数
        * window.opener.父页面的函数

* **JS的window对象的常用属性**
    * 地址栏属性
        * location
            * window.location.href="URL"
            * window.location.reload()  //重新加载
    * 历史记录属性
        * history
            * window.history.forward()  //页面前进
            * window.history.back() //页面回退
            * window.history.go(index)  //跳转到指定的页面
            window.history.go(0)相当于刷新
    * 屏幕属性
        * screen
            * width
            window.screen.width
            * height
            window.screen.height
    * 浏览器配置属性
        * navigator
            * agent
            * ...

* **document对象学习**
    * document对象的概念
        * 浏览器对外提供的支持js的用来操作HTML文档的一个对象，此对象封存的HTML文档的所有信息

    * 使用Document
        * 获取HTML元素对象
        1. 直接获取方式：
            * 通过id
            * 通过name属性值
            * 通过标签名
            * 通过class属性值
        2. 间接获取方式：
            * 父子关系
                var children = 对象名.childNodes;
            * 子父关系
                var parent = 对象名.parentNode;
            * 兄弟关系
                var preEle = *.previousSibling;
                var nextEle = *.nextSibling;

        * 操作HTML元素对象的属性
        1. 获取元素对象
        2. 操作元素属性
            * 获取
            元素对象名.属性名   //---固有
            元素对象名.getAttribute("属性名");  //返回自定义属性的值
            * 修改 
            元素对象名.属性名
            元素对象名.setAttribute("属性名","属性值");
            * **注意：** 尽量不要修改id和name属性

        * 操作HTML元素对象的内容和样式
        1. 操作元素内容
            * 获取
                * 元素对象名.innerHTML  //获取所有内容
                * 元素对象名.innerText  //获取文本内容
            * 修改
                * 元素对象名.innerHTML = 值     //会将原有内容覆盖
        2. 操作元素样式
            * 获取元素对象
                * 通过style属性
                元素名.style.属性名=值
                * 通过className
                元素对象名.className=值

        * 操作HTML的文档结构
            * 增加节点
            * 删除节点
                * innerHTML
                * 父节点.removeChild(子节点对象)    //删除指定的子节点 
                * **代码**
                ```
                function uploadMore(){
                    var showdiv = document.getElementById("");
                    //获取存放的div
                    var inp = document.createElement("input");
                    inp.type = "file";
                    //创建文件上传的input
                    var btn = document.createElement("input")
                    btn.type = "button";
                    btn.value = "删除"
                    //创建删除按钮
                    btn.onclick = function(){
                        showdiv.removeChild(inp);
                        showdiv.removeChild(btn);
                        showdiv.removeChild(br);
                    }
                    //删除按钮功能实现
                    var br = document.createElement("br");
                    //换行
                    showdiv.append(inp);
                    showdiv.append(btn);
                    showdiv.append(br);
                    //追加到div中
                }
                ```

        * document操作form元素
            1. 获取form表单对象
                * 使用id
                var fm = document.getElementById("fm");
                * 使用name属性
                var fm = document.fm;
            2. 获取form表单下所有表单元素集合
                * fm.elements;
            3. form表单的常用方法
                * fm.submit();
                * fm.reset();
            4. form的属性操作
                * 表单对象名.action="";
                * 表单对象名.method="";
            5. JS 表单元素的通用属性
                * 只读模式
                readonly = "readonly";
                * 关闭模式   
                disabled = "disabled";

        * document操作表单元素
            1. JS 操作多选框
                * 选中状态true，未选中状态为false（checked）
            2. JS 操作下拉框
                * 选中状态true，未选中状态为false（selected）

        * document对象实现form表单校验
            1. 正则表达式
            2. 失去焦点事件
            3. 输入密码框调用确认密码框的事件
            4. 使用return结束
            5. 每个校验使用返回值，再使用阻断事件达到整体校验合格才能提交的效果


### 16. 模拟淘宝

### 17. JS 操作表格
* **删除table的行**
    * 表格对象.deleteRow(行对象.rowIndex)
    * 行对象 = button.parentNode.parentNode;
    