## 类
        类的构成
        类(Class) 由3个部分构成
            类的名称:类名
            类的属性:一组数据
            类的方法:允许对进行操作的方法 (行为)
                例：人类设计,只关心3样东西:
                事物名称(类名):人(Person)
                属性:身高(height)、年龄(age)
                方法(行为/功能):跑(run)、打架(fight)
        定义类    
        class 类名:
            方法列表（方法参数地方写self）
         
## 对象
        创建对象
            创建对象
                创建对象的格式为:
                对象名 = 类名()
                对象的调用及属性的添加
        方法
            __init__方法
                <1>使用方式
                def 类名:
                    #初始化函数，用来完成一些默认的设定
                    def __init__(参数):
                        pass
                <2>__init__()方法的调用

                # 定义汽车类
                class Car:
                    def __init__(self):
                        self.wheelNum = 4
                        self.color = '蓝色'
                demo：
                class Car:
                    def __init__(self,new_wheelNum,new_color):
                        self.wheelNum = new_wheelNum
                        self.color = new_color
                    1. 打印id()             print("tom")---> 打印tom在内存中地址
                    2. 定义__str__()方法                       当使用print输出对象的时候，只要自己定义了__str__(self)方法，那么就会打印从在这个方法中return的数据    return什么就打印什么

## 正则表达式
        正则表达式是一个特殊的字符序列，它能帮助你方便的检查一个字符串是否与某种模式匹配。
        re 模块使 Python 语言拥有全部的正则表达式功能。
        
## re模块
        re.match函数
        re.match 尝试从字符串的起始位置匹配一个模式，如果不是起始位置匹配成功的话，match()就返回none。  re.match(pattern, string, flags=0)
        
        re.search方法
        re.search 扫描整个字符串并返回第一个成功的匹配。
        re.search(pattern, string, flags=0)
        
        Python 的 re 模块提供了re.sub用于替换字符串中的匹配项。
        re.sub(pattern, repl, string, count=0, flags=0)
        
        re.compile 函数
        compile 函数用于编译正则表达式，生成一个正则表达式（ Pattern ）对象，供 match() 和 search() 这两个函数使用。
        re.compile(pattern[, flags])
        
        findall
        在字符串中找到正则表达式所匹配的所有子串，并返回一个列表，如果没有找到匹配的，则返回空列表。
        注意： match 和 search 是匹配一次 findall 匹配所有。
        findall(string[, pos[, endpos]])
        
        正则表达式对象
        re.RegexObject
        re.compile() 返回 RegexObject 对象。

        re.MatchObject
        group() 返回被 RE 匹配的字符串。
        
## datetime模块学习
        如Task4
    
## http请求
        可使用requests模块或urllib、urllib2模块