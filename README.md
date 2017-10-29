#泥巴实习总结1.0 
##Linux环境搭建
1. 下载Ubuntu ISO文件
2. 通过大白菜制作Ubuntu启动盘
3. 自定义安装Ubuntu系统，释放硬盘空间，在释放的空间中安装Ubuntu。
4. 更新本系统的源
5. 安装vim
6. 更新源（网易 阿里等）
##安装所需软件
1. 安装VScode编译器
2. 注册GitHub账号，并建立库
3. 将VScode与GitHub互联，实现本地库文件上传
4. 在VScode上安装Markdown插件
##英语学习
1. 安装英语流利说APP
2. 通过英语流利说学习英语，每天至少5分钟
3. 每天学习完成后进行打卡
##编程学习
1. HTML+CSS
*   CSS边框属性 style、color、width
*   应用多个class到一个元素，只需要在多个class之间用空格分开
*   border-radius:50% //改变边框为圆角
*   使用html5技术把表单设置为必填
    <input type="text" required>
*   css处理样式覆盖
    body ---> class1 ---> class2 ---> ID ---> 内联样式 ---> Important
*   RGB具有与十六进制代码完全相同数量的可能值
2. JavaScript
*   .length   //获取字符串的长度
*   []    //使用中括号获取字符串中的第一个字符
*   .length -1 //使用中括号索引查找字符串的最后一个字符
*   当使用[]去访问数组的时候，第一个[index]访问的是该数组中的第N个数组，第二个[index]访问的是第N个子数组的第N个元素
    例：var maData=myArry[2][1];
*   push函数--追加数组数据
    例：myArry.push(["dog",3]);
*   pop函数--弹出数组最后数据
    例：var oneDown=[1,4,6].pop();
    result--->[1,4]
*   shift()函数--移出数组第一个数据
    例：var oneDown=myArry.shift();
*   unshift()函数--移入数据到数组第一位
    例：var myArry=[["john",23],["dog",23]];
        var myArry.shift();
        myArry.unShift(["Paul",35]);
*   与字符串数据不可变不同，数组的数据是可以改变的，并可以自由改变--使用索引修改数据组中的数据
3. JavaScript函数定义
*   把代码重复的部分抽取出来，放到一个函数function中。
    例：function myFunction(){
        console.log("Hi World");
    }
    myFunction();
    result--->Hi World
*   作用域影响着变量的作用范围，在函数外定义的变量具有全局作用域。具有全局作用域的变量可以在代码的任何地方被调用。
    没有使用var关键字的变量，会被自动创建在全局变量作用域中，变成全局变量。
*   一个程序中可能具有相同名称的局部变量和全局变量，在这种情况下局部变量会优先于全局变量。
*   运算符
    与相等运算符不同的是全等运算符比较严格，它会同时比较元素的值和数据类型。
    例：1=='1' // true  
    1==='1' // false
*   JavaScript对象操作
    对象和数组很相似，数组是通过索引来访问和修改数据的，对象是通过属性来访问和修改数据的。
    var cat={
        "name":"xiaomao",
        "legs a":4,
    };
*   使用点操作符读取对象属性
    var first=cat.name;
*   如果访问的属性名称有空格，这时只能用中括号操作符([])。
    var first=cat["legs a"];
    
        