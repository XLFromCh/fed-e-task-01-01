# fed-e-task-01-01

1、 输出结果:9
    原因：var定义变量的时候发生了变量提升，所以变量i是一个全局变量，当循环执行完毕之后i的值为9

2、输出结果：tmp is not defined
    原因：花括号内let定义了同名变量，因此在代码块中的tmp变量指的是let定义的变量。又因为console语句在定义变量之前，此时代码会认为没有声明tmp这个变量	

3、ler minNumber=arr.reduce((res,item)=>res<item?res:item,arr[0])

4、var关键字有声明提升的现象，且声明的变量为全局变量
   let关键字声明变量作用域为当前代码块内
   const关键字一般用于声明常量，声明的变量不允许修改

5、输出结果20
   箭头函数的this指向行文上下文，所以此时的this指向obj对象

6、可以用来定义对象内的私有属性

7、浅拷贝只复制了对象的指针地址，因此修改浅拷贝两个对象中任意一个对象时，另外一个对象也会跟随改变
   深拷贝复制了对象内的值，所以修改其中一个对象的时候不会影响另外一个对象

8、js是一门单线程语言，异步编程可以让js不必等待需要较长运行时间的代码执行完毕，先执行其他同步代码。等异步代码返回结果之后再执行异步代码。
EventLoop是浏览器中的任务队列机制。常见微任务有process.nextTick、promise、MutationObserver。宏任务有普通script代码、setTimeout、setInterval 、setImmediate等。
浏览器先执行同步代码，这属于宏任务，并把微任务放入微任务栈中。执行完同步代码之后再执行微任务栈中的代码。执行完毕之后渲染页面，之后再次开始执行下一轮 Event Loop中的宏任务（setTimeOut等）

9、new Promise((resolve)=>{
            resolve('hellow')
        }).then(res=>{
            return res+'lagou'
        }).then(res=>{
            console.log(res+'i love you')
        })

10 TS是JS的一个超集，ts包含了js，并加强了类型检查、类、接口等内容

11、优点：1.避免了动态类型带来的代码混乱，而且在代码执行前就能发现类型问题导致的bug
	  2.有利于团队规范项目中的类以及类的属性
    缺点：1.较高的学习成本
	  2.小型项目中导致代码冗余，不够灵活			
	
	
