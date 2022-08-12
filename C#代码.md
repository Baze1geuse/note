# C#代码

## 打印字符
`Console.WriteLine("字符");`（自动换行）
`Console.Write("字符");`  （不换行）
特殊打印，如：
`Console.WriteLine("字符" + 数字);`
结果为：`字符数字`两者连在一起


## 输入字符，回车结束
`Console.ReadLine();`


## 等待键盘输入一个按键
`Console.ReadKey();`


## 定义类型
整数
`int`

单精度浮点数
`float`
float类型赋值时须在数值后加f，否则会被视为双精度浮点型
例：`float a = 3.14f;`

双精度浮点数
`double`

字符串
`string`

布尔数
`bool`
仅有ture和false


## 转换类型
`Convert.To类型名(被转换变量名);`



## 字符串格式化
加号拼接
`Console.WriteLine("a=" + 3 + ",b=" + 34);`

序号占位符
```
string fruit = "水果";
Console.WriteLine("{0}吃了{1}", "我"， fruit);
```

利用$字符串格式化
```
string game = "黑魂";
float score = 9.5f;
Console.WriteLine($"{game}在某网站的评分为{score}");
```


![字符串格式化常用方法优缺点.png](../_resources/字符串格式化常用方法优缺点.png)



## 字符串构造
`string.Format("字符串");`


## 特殊字符
换行符
`\n`

制表符
`\t`

符号文本
`\符号`
例：`\"`
文本结果为："


## 替换字符串
`string.Replace`


## 布尔运算
算数判断
`>`
`<`
`>=`
`<=`
`==`
`!=`

逻辑连接
`&&`
`||`

ture和false颠倒
`!`

## 随机数发生器
```
Random random = new Random();
int r = random.Next(0, 100);
```


## 分析输入是否为数字
`bool b = int.TryParse("输入字符", out n);`
返回值b为一个布尔数即ture或false，当b为ture时n为输入值，当b为false时n无法读取