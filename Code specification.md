# Code specification

## Git提交规范

每个类型值都表示了不同的含义，类型值必须是以下的其中一个：

- feat：提交新功能
- fix：修复了bug
- docs：只修改了文档
- style：调整代码格式，未修改代码逻辑（比如修改空格、格式化、缺少分号等）
- refactor：代码重构，既没修复bug也没有添加新功能
- perf：性能优化，提高性能的代码更改
- test：添加或修改代码测试
- chore：对构建流程或辅助工具和依赖库（如文档生成等）的更改

#### EX

    feat: add xxx function
    fix: xxx function yyy question

## 命名规范

### *匈牙利命名法*

该命名规范，要求前缀字母用变量类型的缩写，其余部分用变量的英文或英文的缩写，单词第一个字母大写。

#### Ex

```cpp
int iMyAge;        #  "i": int
char cMyName[10];  #  "c": char
float fManHeight;  #  "f": float
```

#### 其他

前缀类型还有：

```text
a      数组（Array）
b      布尔值（Boolean）
by     字节（Byte）
c      有符号字符（Char）
cb     无符号字符（Char Byte，并没有神马人用的）
cr     颜色参考值（Color Ref）
cx,cy  坐标差（长度 Short Int）
dw     双字（Double Word）
fn     函数（Function）
h      Handle（句柄）
i      整形（Int）
l      长整型（Long Int）
lp     长指针（Long Pointer）
m_     类成员（Class Member）
n      短整型（Short Int）
np     近程指针（Near Pointer）
p      指针（Pointer）
s      字符串（String）
sz     以 Null 做结尾的字符串型（String with Zero End）
w      字（Word）
```

### *驼峰式命名法*

驼峰式命名法，又叫小驼峰式命名法。

该命名规范，要求第一个单词首字母小写，后面其他单词首字母大写，简单粗暴易学易用。

#### Ex

```cpp
int myAge;
char myName[10];
float manHeight;
```

### *帕斯卡命名法*

帕斯卡命名法，又叫大驼峰式命名法。

与小驼峰式命名法的最大区别在于，每个单词的第一个字母都要大写。

#### Ex

```cpp
int MyAge;
char MyName[10];
float ManHeight;
```

### *下划线命名法*

尤其在宏定义和常量中使用比较多，通过下划线来分割全部都是大写的单词。

该命名规范，也是很简单，要求单词与单词之间通过下划线连接即可。

#### Ex

```cpp
int my_age;
char my_name[10];
float man_height;
```

---

参考文献：

[Git提交规范](https://zhuanlan.zhihu.com/p/67804026)

[四种基本的编程命名规范（匈牙利命名法、驼峰式命名法、帕斯卡命名法、下划线命名法） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/89909623)
