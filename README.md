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
*   与字符串数据不可变不同，数组的数据是可以改变的，并可以自由改变--使用索引
