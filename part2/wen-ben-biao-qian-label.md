# 文本标签 Label

---

##### 作用：文本显示

### 设计属性

* ##### 对象名称

  * 类型：字符串；

  * 值：

  * 说明：自定义控件对象名；
* ##### 文本

  * 类型：字符串；

  * 值：

  * 说明：默认显示的文本；
* ##### 文本显示行数

  * 类型：数值；

  * 值：默认：空；

  * 说明：为指定宽高的文本标签设置显示行数，显示不完全的内容以省略号代替。PC端设置数字后只会显示一行；
* ##### 图片选择

  * 类型：按钮；

  * 值：选择图片、清除图片；

  * 说明：设置显示图片地址；
* ##### 数据域

  * 类型：字符串；

  * 值：

  * 说明：符合变量命名规则；数据域作为表单上下文的一个属性，所有指定数据属性的控件的值，都会保存在数据域对象中；
* ##### 数据属性

  * 类型：字符串；

  * 说明：符合变量命名规则；用于获取控件的值；控件的值会保存在表单上下文对象的数据属性上，如果指定了数据域，则会保存在数据域对象上；
* ##### 绑定路径

  * 类型：字符串；

  * 说明：为控件赋值的属性；页面加载时，会从表单的数据上下文对象DataContext中获取相应字段值进行显示；
* ##### 数据格式

  * 类型：字符串；

  * 说明：设置显示文本的格式；

    1、控制显示的小数位数：\#\#0.00；

    2、日期时间：yyyy-MM-dd HH:mm:ss；

    3、日期：yyyy-MM-dd；

    4、时间：hh:mm:ss；

    5、货币：C
* ##### 可用-设置控件是否可用；
* ##### 可见：设置控件是否显示；
* ##### 只读：设置文本输入框是否只读，不允许编辑；

### 事件处理程序

* ##### Click

  * 调用时机：用户点击控件时；
  * 说明：
  * 备注：

### 属性、方法

* ##### Text-属性，设置或获取控件显示的字符串；

  * 说明：字符串类型；
* * 示例：
  * ```js
    Label.Text = '姓名'
    ```



