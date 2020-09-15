

## 结构体 structure vs 类 class

- 相似点：

  - 用关键字struct声明的自定义数据类型

  - 与类相似，可含：**构造函数，常数，字段，方法，属性，索引器，运算符和嵌套类型等**

- 不同点：

  - 对于结构中的**实例字段 field**成员，不能在声明时赋值初始化
  
  - 结构体声明后，可以使用new创建构造对象，也可以不。如果不，在初始化所有fields之前，field将保持**未赋值状态**且对象**不可用**
  
  - **结构体不支持继承，不能作为一个类的基类，但结构体从*基类object*继承，结构体也可以实现接口**
  
  - 结构体是**值类型**(在堆栈中创建) vs 类是 **引用类型**
  
    - 结构体是值类型：影响性能，可正面可负面。正：分配空间快，将内联或保存在堆栈中，可以直接当参数来传递，可以A=B就使得**结构体**所有内容被复制(性能损失)，但是**类**却只复制**引用**，
    所以当传参的时候，只传递结构体在内存中的地址，速度就与类一样快了。
    
    - 默认的访问权限:struct默认public，class默认private
  