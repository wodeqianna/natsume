# 泥巴实习总结1.0 
## Linux环境搭建
1. 下载Ubuntu ISO文件
2. 通过大白菜制作Ubuntu启动盘
3. 自定义安装Ub  untu系统，释放硬盘空间，在释放的空间中安装Ubuntu。
4. 更新本系统的源
    sodu apt-get update
5. 安装vim
    sudo apt-get install vim-gtk
6. 更新源（网易 阿里等）
    $sudo gedit /etc/apt/sources.list
    复制粘贴新的源
    sodu apt-get update
## 安装所需软件
1. 安装VScode编译器
    安装js--->sudo apt install nodejs-legacy
    node -v //检查是否安装成功 
2. 注册GitHub账号，并建立库
3. 将VScode与GitHub互联，实现本地库文件上传
安装get---> sudo apt-get install git
git config --global user.name "你的github用户名"
git config --global user.email "你的github邮箱地址"
4. 在VScode上安装Markdown插件
在扩展上下载 Markdown Preview Enhanced
## 英语学习
1. 安装英语流利说APP
2. 通过英语流利说学习英语，每天至少5分钟
3. 每天学习完成后进行打卡
## 编程学习
1. HTML+CSS
*   CSS边框属性 style、color、width
*   应用多个class到一个元素，只需要在多个class之间用空格分开
*   border-radius:50% //改变边框为圆角
*   使用html5技术把表单设置为必填
    ```<input type="text" required>```
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
    例：
    ```
    function myFunction(){
    console.log("Hi World");
    }
    myFunction();
    ```
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

*   中括号操作符的另一个使用方式是用变量来访问一个属性，当你需要遍历对象的属性列表或查表时，这种方式极为有用。
    var testobj={
        12:"Namath";
        16:"Montana";
        19:"Vnitas";
    };
    var playNumber=16;
    var player=testobj[playNumber];
*   使用rondom()生成随机小数
    Math.rondom()用来生成一个在0-1(不包括1)之间的随机数.因此Math.rondom()可能返回0但绝对不会返回1。
    例:生成一个0-9之间的随机整数
    return Math.floor(Math.random()*10);
 4. 基本算法
*   翻转字符串算法挑战
方法一
使用split()将字符串分割成数组
使用reverse()将数组进行翻转
使用join()将数组转化为字符串
 ```
function reverseString(str) {
var new1=str.split('');
var new2=new1.reverse();
var new3=new2.join('');
return new3;
}
reverseString("hello");
 ```
方法二
将字符串进行反向遍历
 ```
function reverseString(str) {
var new1="";
for (var i = str.length-1; i>=0 ; i--) {
    new1+=str[i];
}
return new1;
}
reverseString("hello");
 ```
*   阶乘算法挑战
方法一
使用for循环进行阶乘
 ```
function factorialize(num) {
    var sum=1;
    for (var i = num; i>0 ; i--) {
        sum*=i;
    }
return sum;
}
factorialize(5);
 ```
*   回文算法挑战
方法一
使用toLowerCase()将字符串转化为小写
正则表达式 
\W表示：元字符用于查找非单词字符
var reg=/[\W\_]/g;
使用replace()替换与正则表达式匹配的子串
 ```
function palindrome(str) {
var str1=str.toLowerCase();
var reg=/[\W\_]/g;
var str2=str1.replace(reg,"");
var str3=str2.split("");
var str4=str3.reverse();
var str5=str4.join("");
return str2 === str5;
}
palindrome("eye");
 ```
* 寻找最长的单词算法挑战
利用split()方法将字符串分成每个单词组成的数组，取得其中最长的长度
 ```
function findLongestWord(str){
var max = 0;
var arr = str.split(' ');
for(var i=0;i<arr.length;i++){
max = arr[i].length>max?arr[i].length:max;
}
return max;
}
findLongestWord("The quick brown fox jumped over the lazy dog");
 ```
*   设置首字母大写算法挑战
toUpperCase() 方法用于把字符串转换为大写。
slice() 方法可从已有的数组中返回选定的元素。
 ```
function titleCase(str) {
    var arr,upChar;
    str = str.toLowerCase();
    arr = str.split(' ');
    for(var i=0;i<arr.length;i++){
        upChar =  arr[i][0].toUpperCase();
        arr[i] = upChar + arr[i].slice(1);
    }
    arr = arr.join(' ');
    return arr;
} 
```
*   寻找数组中的最大值算法挑战
使用到了二维数组的遍历
 ```
 function largestOfFour(arr) {
    var one=[0,0,0,0];  
    for (var i = 0; i < arr.length; i++) {
        for (var j = 0; j < arr[i].length; j++) {
            if (one[i]<arr[i][j]) {
                 one[i]=arr[i][j]
            }
        }
    }
return one;
}
largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]); 
```
*   确认末尾字符算法挑战
检查一个字符串(str)是否以指定的字符串(target)结尾。
如果是，返回true;如果不是，返回falsev.
```
function confirmEnding(str, target) {
    var alen=str.substr(-target.length);
    if (alen==target) {
        return true;
    }else{
        return false;
    }
}
confirmEnding("He has to give me a new name", "name");

```
*   重复操作算法挑战
重复一个指定的字符串 num次，如果num是一个负数则返回一个空字符串
```
function repeat(str, num) {
    var result = '';
    if(num<0){
        return '';
    }else{
    for(var i=0;i<num;i++){
        result += str;
            }
    }
return result;
}
```
*   字符串截取算法挑战
```
function truncate(str, num) {
    var result;
            if(num<=3){
                result = str.slice(0,num) +'...';
            }else if(str.length>num){
                result = str.slice(0,num-3) + '...';
            }else{
                result = str;
            }
            return result;
        }
truncate("A-tisket a-tasket A green and yellow basket", 11);
```
*   数组分割算法挑战
push() 方法可向数组的末尾添加一个或多个元素，并返回新的长度
```
function chunk(arr, size) {
    var result=[];
    var a=[];
    for (var i = 0; i < arr.length; i++) {
        a.push(arr[i]);
        if (((i+1)%size==0||i==arr.length-1)) {
            result.push(a);
           a=[]; 
        }
    }
    return result;
        }
chunk(["a", "b", "c", "d"], 2);

```
*   数组截断算法挑战
返回一个数组被截断n个元素后还剩余的元素，截断从索引0开始
同样用到push() 方法

```
function slasher(arr, howMany) {
var result=[];
for (var i = howMany; i < arr.length; i++) {
    result.push(arr[i]);
}
return result;
}
slasher([1, 2, 3,4], 2);
```
*   数组查询算法
indexOf() 方法可返回某个指定的字符串值在字符串中首次出现的位置
```
function mutation(arr) {
    var arr1 = arr[0].toLowerCase();
    var arr2 = arr[1].toLowerCase();
    for(var i=0;i<arr[1].length;i++){
        if(arr1.indexOf(arr2[i]) == -1){
            return false;
        }
    }
    return true;
}
mutation(["hello", "hey"]);
```
*   删除数组中特定值算法挑战
```
function bouncer(arr) {
        for(var i=0;i<arr.length;i++){
            if(!arr[i] == true){
                arr.splice(i,1);
                i--;
            }
        }
        return arr;
    }
bouncer([7, "ate", "", false, 9]);
```