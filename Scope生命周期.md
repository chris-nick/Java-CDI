## Scope 生命周期

1. Application生命周期
    即web application启动后，处于该生命周期的对象或变量将一直存在，直到web应用停止或重新启动。通常用来做网站计数器或实现流量访问之类。
    
2. Session生命周期
    每次我们在某种类型的浏览器(比如:IE或Firefox)里，请求web-application的某个页面时，就会生成Session，
    <b><font color="red">只要浏览器不关闭</font></b>，Session就能持续有效。说得更白一点：按F5刷新，该对象/变量不会被自动销毁，除非Session过期。
    注：Session是跟浏览器有关的，如果在FireFox里打开web Application的某个url，再到IE里打开同样的url，这二个浏览器里的Session是不同的。

3. Request生命周期
    即：只有本次http请求才有效，通俗点讲，如果你定义一个变量的生命周期是Request级别，刷新一次页面后，该变量就被初始化(重新投胎)了。
