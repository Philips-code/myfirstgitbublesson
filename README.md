# myfirstgitbublesson
following the guide of the github to creat a new github
是对自己查阅资料的一个总结，可能有不足之处。欢迎转载，请注明出处。

prototype
prototype属性在javascript中是函数独有的。为什么要设置这个属性，看完下文阮一峰的追根溯源之后，应该会有了解。
Javascript继承机制的设计思想  摘录出其中最重要的一段话。
Brendan Eich决定为构造函数设置一个prototype属性。这个属性包含一个对象（以下简称"prototype对象"），所有实例对象需要共享的属性和方法，都放在这个对象里面；那些不需要共享的属性和方法，就放在构造函数里面。
总结：prototype是构造函数的一个属性，这个属性里面包含一个对象，就是我们常说的原型对象，它的作用是存放所有实例对象需要共享的属性和方法。
__proto__
当调用构造函数创建一个新实例后，该实例的内部将包含一个指针（内部属性），指向该函数的原型对象。这个连接存在于实例和构造函数的原型对象之间，而不是存在于实例和构造函数之间。
__proto__和[[prototype]]，其于实是说的一回事。不过是从两个角度来看待这件事而已。
__proto__是每个对象都有的属性。



JavaScript中，Object.prototype是所以对象的顶层。所有对象都会从它的原型上继承一个 constructor 属性。

Function的构造器指向自己，Object的构造器指向Function，这个也好理解，Object也是一个构造函数，自然他也是一个Function对象所有对象都会有一个[[prototype]]属性


参考书籍：
《javascript高级程序设计第三版》《你不知道的javascript 上》《你不知道的javascript 中》
《你不知道的javascript 下》
