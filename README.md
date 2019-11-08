# JSONDemo

##.json解析：（JavaScrip tObject Notation）-js对象表示法 见仓库JSONDemo
    
    1.是一种轻量级的数据交换格式：
    2.类似xml，更小，更快，更易解析
    3.最早使用与javascript，容易解析，最后推广到全语言
    4.发展历程：
        1998年：w3c推出xml
        2002:年：发明json
        2006年：普及json，因为xml太笨重，处理麻烦，json更小，更轻量
    5.json处理：
        1.java本身没有处理json的包：
        2.处理包：
            1.org.json:json官方推荐的解析类
                -简单易用，通用性强
                -复杂功能欠缺
            2.Gson：google出品
                -基于反射，可以实现json对象，json字符串和java对象互转
            3.jackson：号称最夸的json处理器
                -简单易用，社区更新和发布速度比较快
    6.主要用途：
        1.json生成：
        2.json解析：
        3.json校验：
        4.和java Bean对（pojo）象互相转换
            -有无参构造函数
            -private属性
            -属性get set方法
    7.json和xml比较
        1.都是数据交换格式，可读性强，可拓展新高
        2.大部分情况下，json更有优势，编码简单，转换方便，而且json字符串长度一般小于xml，传输效率更高
        3.xml更加注重标签和顺序，json会丢失信息：
            <expression>
                <operand>a</operand>
                <operator>+<operator>
                <operand>b</operand>
            <expression>
            将以上数据，放到一些开源的xml to json工具上测试得到
            {
                "expression":{
                    "operand":["a","b"]
                    "operator":"+"
                }
            }
            将数据回转得到:
            <expression>
               <operand>a</operand>
               <operand>b</operand>
               <operator>+<operator>
            <expression>   
            由上可知：当转换时，json就会丢失顺序，所以如果数据传输要保证顺序，尽量使用xml
        
   
