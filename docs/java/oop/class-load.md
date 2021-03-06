# 类加载机制

**类的加载是指将类的相关信息加载到内存，类是动态加载的，当第一次使用这个类的时候才会加载。加载一个类时，会看其父类是否已加载，如果没有，则会加载其父类。**

## 类的信息

- 类变量（静态变量）
- 类初始化代码
  - 定义静态变量时的赋值语句
  - 静态初始化代码块
- 类方法（静态方法）
- 实例变量
- 实例初始化代码
  - 定义实例变量时的赋值语句
  - 实例初始化代码块
  - 构造方法
- 实例方法
- 父类信息引用

## 类加载过程

- 分配内存保存类的信息
- 给类变量赋默认值
- 加载父类
- 设置父子关系
- 执行类初始化代码

**类初始化代码是先执行父类的，再执行子类的。父类执行时，子类静态变量的值是默认值。**

**加载一个类时，会看其父类是否已加载，如果没有，则会加载其父类。**

## 内存空间

- 栈

存放函数的局部变量和引用

- 堆

存放动态分配的对象

- 方法区

存放类的信息