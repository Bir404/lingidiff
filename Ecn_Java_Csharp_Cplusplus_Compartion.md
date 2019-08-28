# 易语言.飞扬”与 JAVA、C#、C++ 的异同：

| **易语言****.****飞扬** | **JAVA**                                                     | **C#**                                                       | **C++**                             |                                                              |
| ----------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ----------------------------------- | ------------------------------------------------------------ |
| 编译                    | 编译为机器码                                                 | 编译为字节码                                                 | 编译为字节码                        | 编译为机器码                                                 |
| 执行                    | 由CPU直接执行                                                | 在虚拟机中执行                                               | 在虚拟机中执行                      | 由CPU直接执行                                                |
| 面向对象                | 完全面向对象                                                 | 完全面向对象                                                 | 完全面向对象                        | 支持面向对象                                                 |
| 垃圾回收                | 支持                                                         | 支持                                                         | 支持                                | （目前）不支持                                               |
| 标准类库                | 有，有待丰富                                                 | 非常丰富                                                     | 非常丰富                            | 标准类库较小，但第三方类库非常丰富                           |
| 单根继承                | 是  所有类都是“系统.对象”的子类                              | 是  所有类都是“java.lang.Object”的子类                       | 是  所有类都是“System.Object”的子类 | 否  任何类都可以有多个基类，没有固定基类                     |
| 跨平台                  | 支持  同一个源代码未经修改或经少量修改可在其它平台下编译运行 | 支持  同一个程序或类库未经修改或经少量修改可在其它平台下运行 | 不支持  仅限于Windows平台           | 支持（但在多线程、网络、文本编码转换等领域需第三方类库支持） |
| 多线程                  | 支持                                                         | 支持                                                         | 支持                                | 第三方类库支持                                               |
| Unicode                 | 支持                                                         | 支持                                                         | 支持                                | 部分支持                                                     |
| 网络                    | 支持                                                         | 支持                                                         | 支持                                | 第三方类库支持                                               |
|                         |                                                              |                                                              |                                     |                                                              |
| 语言复杂度              | 简单                                                         | 较简单                                                       | 较简单                              | 较复杂                                                       |
| 学习难度                | 容易                                                         | 较容易                                                       | 较容易                              | 较难                                                         |
| IDE支持                 | 自行开发，会支持很好                                         | 支持很好                                                     | 支持很好                            | 支持较好                                                     |



| **易语言****.****飞扬**       | **JAVA**                            | **C#**                                               | **C++**                                |                                                              |
| ----------------------------- | ----------------------------------- | ---------------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
| 启动方法                      | 公开 静态 整数 启动(文本[] 参数)    | public static void main(String[] args)               | public static void Main(string[] args) | int main(int argc, char** argv)                              |
| 启动类                        | 编译时指定                          | 在 MANIFEST.MF 文件中指定                            | Main方法所属类                         | 无                                                           |
| 基本类型                      | 整数，小数，逻辑，文本，字节集      | byte, short, int, float, double, boolean, long ,char |                                        | char, unsigned char,short, unsigned short, int, unsigned int, long, float, double, bool |
| 定义类时所用关键字            | 类 或 class                         | class                                                | class                                  | class                                                        |
| 公开/保护/私有 所对应的关键字 | 公开/扩展/私有                      | public/protected/private                             | public/protected/private               | public/protected/private                                     |
| 定义变量                      | 整数 i = 123;  或  int i = 123;     | int i = 123;                                         | int i = 123;                           | int i = 123;                                                 |
| 定义数组变量                  | 整数[] a = { 1, 2, 3 };             | int[] a = { 1, 2, 3 };                               | int[] a = { 1, 2, 3 };                 | int[] a = { 1, 2, 3 };                                       |
| 定义类                        | 公开 类 我的类 <基类型 = XXX>  {  } | public class MyClass extends XXX  {  }               | public class MyClass : XXX  {  };      | class MyClass :public XXX  {  };                             |



| **易语言****.****飞扬** | **JAVA**                             | **C#**                                                    | **C++**                                                   |                                                           |
| ----------------------- | ------------------------------------ | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| 定义接口                | 公开 接口 我的接口  {  }             | public interface MyInterface  {  }                        | public interface MyInterface  {  };                       | 没有明确的接口概念，但可用纯虚类加多重继承达到接口的效果  |
| 定义枚举                | 公开 枚举 我的枚举  {  u, v, w  }    | public enum MyEnum  {  u, v, w  }                         | public enum MyEnum  {  u, v, w  };                        | enum MyEnum  {  u, v, w  };                               |
| 创建对象                | 对象 obj = 创建 对象();              | Object obj = new Object();                                | Object obj = new Object();                                | MyClass obj;  或  MyClass* pObj = new MyClass();          |
| 创建数组对象            | 整数[] a = 创建 整数[x];             | int[] a = new int[x];                                     | int[] a = new int[x];                                     | int* a = new int[x];                                      |
| 条件判断（if）          | 如果( 1 + 1 == 2)  {  }  否则  {  }  | if( 1 + 1 == 2)  {  }  else  {  }                         | if( 1 + 1 == 2)  {  }  else  {  }                         | if( 1 + 1 == 2)  {  }  else  {  }                         |
| 多条件判断（switch）    | 假如(x)  {  为 1:  为 2:  为其他:  } | switch(x)  {  case 1: break;  case 2: break;  default:  } | switch(x)  {  case 1: break;  case 2: break;  default:  } | switch(x)  {  case 1: break;  case 2: break;  default:  } |
| 循环（while）           | 循环(x < 0)  {  x++;  }              | while(x < 0)  {  x++;  }                                  | while(x < 0)  {  x++;  }                                  | while(x < 0)  {  x++;  }                                  |
| 循环（for）             | C循环(整数 i = 0; i < 10; i++)  {  } | for(int i = 0; i < 10; i++)  {  }                         | for(int i = 0; i < 10; i++)  {  }                         | for(int i = 0;                                            |

