# 条款 1. 仔细区别 pointers 和 references

两者特点

* reference 是另一个对象的别名，因此必须代表某个对象，定义时必须初始化且不能被重新赋值。此外 reference 本身不是一个对象，这一点很重要。
* pointers  是一个指向别的对象的对象，它存储的是另一个对象的地址值，可以被重新赋值。

如何选择

> 当我们知道自己需要指向某个东西，并且绝对不会改变指向其他东西，或者是当实现一个操作符而其语法需求无法由 pointers 达成，则应该选择 references，其他任何时候，采用 pointers。

不太明白，看代码吧： 

* [pointers.cpp](pointers.cpp)
* [references.cpp](references.cpp)


