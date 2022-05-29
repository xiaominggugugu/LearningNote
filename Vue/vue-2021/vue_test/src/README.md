# 总结TOdoList案例

一、组件化编码流程：

​	（1）拆分静态组件：组件要按照功能点拆分，命名不要与 HTML 元素冲突。

​	（2）实现动态组件：考虑好数据的存放位置，数据是一个组件在用，还是一些组件在用：

​	          i. 一个组件在用：放在组件自身即可。

​	          ii. 一些组件在用：放在他们共同的父组件上（**状态提升**）。

二、props适用于：

​	  （1）父组件 ==> 子组件 通信。

​	  （2）子组件 ==> 父组件 通信（要求父组件先给子组件一个函数）。

三、使用 `v-model` 时要切记：v-model 绑定的值不能是 props 传过来的值，因为 props 是不可以修改的！

四、props 传过来的若是对象类型的值，修改对象中的属性时 Vue 不会报错，但是不推荐这样做。