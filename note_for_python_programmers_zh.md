
fast-introduction-for-programmers： Wolfram 语言比 Python 拥有更高级别和更综合化的设计原则，基于完全的符号式语言，以及桌面和云端的无缝操作，和在语言中直接构建的世界最大的算法和数据集成，全部统一的设计和文档，可访问的世界独创笔记本界面，允许更快和更高级开发部署您的理念，无需查找并学习单独的程序库. 从 Wolfram 语言版本 11.2 开始，ExternalEvaluate 框架为包括 Python 在内的其他语言提供了无缝连接，使其能够将您已有的代码和外部程序库融合到 Wolfram 语言中. 开始学习（显示备注）
interactive-usage：您可以交互式使用 Wolfram 语言，如同使用增强版的 Python 交互式 shell，支持即时代码支持、图像、行内界面等.
interactive-usage：Wolfram 语言中的 % 与 Python 交互式 shell 中的 _ 有相同作用.
notebook-documents：Wolfram 笔记本经过了持续三十年以上的开发历程，并且是完整集成与桌面和云端 Wolfram 语言的部分. 它们起到了与 Jupyter 笔记本库的相同作用.
built-in-functions：Wolfram 语言延续了一致统一设计且附带了完整整合的内置函数，而无需从不同设计和约定的不同模块和程序库加载功能.
built-in-functions：在 Wolfram 语言中，函数参数使用方括号 [...] 而不是括号 (...). 括号用于分组.
built-in-functions：Wolfram 语言 语言比 Python 拥有更多且范围广的内置功能，可更简单和快速书写代码，并且 ExternalEvaluate 还可用于整合 Python 代码.
symbolic-expressions：Wolfram 语言的符号表达式提供了一种极其简单的方法在统一的树形结构中表示数据. 其在编程中加入了高等级的自由度，允许对结构和内容进行操作.Python 没有内置的符号功能.
symbolic-expressions：Wolfram 语言表达式的 head 确定数据或表示的操作类型，且可在计算中随时被转换. 所有 Python 对象都有标注的 class 且不能被更改.
symbolic-expressions：Wolfram 语言的符号表达式让程序员可以在其计算中不间断地将未定义变量作为符号使用. 未赋值的变量在 Python 中被认为是 “undefined”，且试图使用未定义变量会造成产生 NameError.
lists：Wolfram 语言列表用大括号 {...} 表示，然而 Python 列表使用相同方括号 [...] 语法同时表示列表和索引. The Wolfram 语言通过用 [[...]] 表示索引来避免混淆，并运用了从 1 而不是从 0 开始的直观的索引系统.
lists：在 Wolfram 语言中，+ 仅仅用于算数加法. 对于字符串串联等使用 <>
lists：跨度在 Wolfram 语言中与 Python 的 : 切片类似，但概化为多维数组.
iterators：这样使用 Table 与在 Python 中使用 [... for ... in ...] 列表推导式结构类型，但有更丰富的语义.
assignments：Wolfram 语言中，延迟赋值生成的变量在你每次使用的时候将动态重新计算其值. 为实现相同功能 Python 则需要使用更复杂的 promise 对象.
assignments：在 Wolfram 语言中的 =. 与 Python 的 del 操作符有相同作用.
assignments：Python 函数创建本地范围变量与 Wolfram 语言中的 Module 类似。
assignments：在 Python 的命名习惯中，大写名称特指分类；在 Wolfram 语言中，大写名称可表示任意类型的内置结构.
patterns：Wolfram 语言的模式语言允许你对任意符号结构的模式进行描述，能够将强大的 regex-like 操作泛用与任意表达式和任意格式的数据.
patterns：在此显示的该类结构的元程序，将代码和数据等同对待，是 Wolfram 语言符号结构的独有特点.
patterns：在 Wolfram 语言模式中的使用与其在 Python 常用表达式中的用法相近. 但是，Wolfram 语言中，| 不仅用于字符串，还可用于任意类型的符号模式匹配.
function-definitions：在 Wolfram 语言的基本函数定义中，参数名称后跟随 _ (“空白”)，允许参数与任意符号式模式一致. 实现了强大且灵活的函数定义，这对于默认的 Python 是不可能的.
function-definitions：在 Wolfram 语言中可使用与 if 语句相同的 /; 应用于函数，允许函数自由根据条件自动选择定义.
function-definitions：Wolfram 语言函数可使用内置的模式匹配来根据其任意参数的符号结构来更改行为. 在 Python 中则需要相对复杂的自定义代码或第三方程序库.
pure-functions:Wolfram 语言中的纯函数与 Python 中的拉姆达表达式工作方法类似.
pure-functions:Wolfram 语言纯函数可以用 # 或给定明确的名称来表示参数. Python 的拉姆达函数则始终需要名称参数.


在 Wolfram 语言中，

函数定义只是给出模式变换规则的赋值.

f[x__,y__]:=x+y



定义一个带有命名为 *x* 和 *y* 的两个参数的函数：

模式代表表达式的类型. 基本的模式结构 _（读作 “blank”）代表任意表达式.
x_（x:_ 的缩写）代表一个模式
__（“两个 blank”） 代表任意表达式序列：
a | b | c 代表 a、b 或 c：
_h 代表任何有标头 h 的表达式：
:> 是一个延迟规则；类似于规则中的 :=
x= 7 “立即” 赋值.
x=:用延迟赋值，当被调用时，值会被重新计算：
x=.清除赋值：

用 Module ()局部化变量：

变量名通常以小写字母为首字母，

大写开头的变量一般是特别为内置对象所保留.

PYTHON 程序员备注：

列表 在 Wolfram 语言中用 {...}

在 Python 的命名习惯中，大写名称特指分类；在 Wolfram 语言中，大写名称可表示任意类型的内置结构.

[列表部分](http://reference.wolfram.com/language/guide/PartsOfExpressions.html)的索引从 1 开始，可以使用 [[[ ... \]]](http://reference.wolfram.com/language/guide/PartsOfExpressions.html) 进行提取：

并运用了从 1 而不是从 0 开始的直观的索引系统.

列表中的 “跨度” 使用 [;;](http://reference.wolfram.com/language/ref/Span.html)

*head*[*arguments*]



Wolfram 语言中的一切都是符号表达式.

Python语言中的一切都是对象.

PYTHON 程序员备注：



Wolfram 语言表达式的 *head* 确定数据或表示的操作类型，且可在计算中随时被转换. 所有 Python 对象都有标注的 *class* 且不能被更改.

完全符号式

[FullForm](http://reference.wolfram.com/language/ref/FullForm.html) 总是显示底层结构.
[Head](http://reference.wolfram.com/language/ref/Head.html) 总是给出一个[表达式](http://reference.wolfram.com/language/guide/Expressions.html)；[Length](http://reference.wolfram.com/language/ref/Length.html) 则给出参数数目.

函数参数始终用逗号分隔.

标准的“迭代器规范”：*min*、*max*、*step*：

迭代器规范只给出一个显式值列表

制作一个嵌套表格：
使用定义f[4,a]
清楚定义:Clear[f]
使用 /; 限制定义，使其只适用于某种条件：
f[x_,y_ ]:=x-y/;x>y


纯函数 匿名函数、拉姆达表达式
Wolfram 语言允许调用 
``& ``纯函数结尾，
``# `` 纯函数第一个参数：

.
创建一个加1的纯函数：


In[1]:=	(#+1)&
Out[1]=	#1
如果纯函数以表达式的标头给出，会对参数应用该函数：
In[2]:=	
Out[2]=	
这是一个具有多个参数的函数：
In[3]:=	
Out[3]=	
可用其它方法指定函数：
In[4]:=	
Out[4]=	

PYTHON 程序员备注： Wolfram 语言纯函数可以用 # 或给定明确的名称来表示参数. Python 的拉姆达函数则始终需要名称参数.

函数应用  视频
将一个函数“映射”到多个表达式是很常见的：

Copy to clipboard.
In[1]:=	
Out[1]=	
PYTHON 程序员备注： Map 在 Wolfram 语言中与 Python 中的 map 相同，除此之外，它可以在任意深度的表达式树上操作.
/@（“斜杠 艾特”）是 Map 的简写形式：

Copy to clipboard.
In[2]:=	
Out[2]=	
这里使用一个 纯函数：

Copy to clipboard.
In[3]:=	
Out[3]=	
Apply 将一个函数应用于多个参数：

Copy to clipboard.
In[1]:=	
Out[1]=	
PYTHON 程序员备注： Apply 在 Wolfram 语言中与 Python 中的拆包操作符 * 类似.
表达式所带的“层”对应于需要提取部分的索引号. 像 Map 这样的函数可以在指定的层进行操作.

PYTHON 程序员备注： “Levels”如同一个数组的维数，但对全部符号表达式进行泛化. Python 的数组函数通常对于一维数组设定.
Map 默认在第一层操作：

Copy to clipboard.
In[1]:=	
Out[1]=	
该操作只在第二层进行：

Copy to clipboard.
In[2]:=	
Out[2]=	
@@ 等价于 Apply，默认在第0层操作：

Copy to clipboard.
In[1]:=	
Out[1]=	
@@@ 是指“在第一层应用”：

Copy to clipboard.
In[2]:=	
Out[2]=	
@ 是指普通函数应用：

Copy to clipboard.
In[3]:=	
Out[3]=	
理解测试
