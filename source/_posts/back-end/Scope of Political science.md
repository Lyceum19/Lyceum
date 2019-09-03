---
title: 'Scope of Political science'
permalink: 'Scope of Political science'
date: 2017-04-15 10:22:05
categories: Sem I
tags:
- Basics of PS
originView: Scope of Political science 
originUrl: 
---
 Now a days, it is very difficult to determine the precise and definite boundaries of political science. It is wide and comprehensive subject and there is no uniformity among political scientists about its scope.  It is the study of organizations and activities of the state, both at national and international levels. It also deals with the distribution of governing power among several agencies by which the actions of the state are determined, expressed, and exercised and with the problems of international life.  Yet some of the important subjects in the scope of political science are given below:-
## 1. Political Science is the Study of State and Government.
Flowing are the points：
![State and Government](http://img.xiangzhangshugongyi.com/DispatcherServlet.png)
这张图片给了我们大概的执行流程：
1. 用户请求首先发送到前端控制器DispatcherServlet，DispatcherServlet根据请求的信息来决定使用哪个页面控制器Controller（也就是我们通常编写的Controller）来处理该请求。找到控制器之后，DispatcherServlet将请求委托给控制器去处理。
2. 接下来页面控制器开始处理用户请求，页面控制器会根据请求信息进行处理，调用业务层等等，处理完成之后，会把结果封装成一个ModelAndView返回给DispatcherServlet。
3. 前端控制器DispatcherServlet接到页面控制器的返回结果后，根据返回的视图名选择相应的试图模板，并根据返回的数据进行渲染。
4. 最后前端控制器DispatcherServlet将结果返回给用户。

## 更具体的流程
上面只是总体流程，接下来我们稍微深入一点，看下更具体的流程，这里没有图，只有步骤解析：
1. 用户请求发送到前端控制器DispatcherServlet。
2. 前端控制器DispatcherServlet接收到请求后，DispatcherServlet会使用HandlerMapping来处理，HandlerMapping会查找到具体进行处理请求的Handler对象。
3. HandlerMapping找到对应的Handler之后，并不是返回一个Handler原始对象，而是一个Handler执行链，在这个执行链中包括了拦截器和处理请求的Handler。HandlerMapping返回一个执行链给DispatcherServlet。
4. DispatcherServlet接收到执行链之后，会调用Handler适配器去执行Handler。
5. Handler适配器执行完成Handler（也就是我们写的Controller）之后会得到一个ModelAndView，并返回给DispatcherServlet。
6. DispatcherServlet接收到Handler适配器返回的ModelAndView之后，会根据其中的视图名调用视图解析器。
7. 视图解析器根据逻辑视图名解析成一个真正的View视图，并返回给DispatcherServlet。
8. DispatcherServlet接收到视图之后，会根据上面的ModelAndView中的model来进行视图中数据的填充，也就是所谓的视图渲染。
9. 渲染完成之后，DispatcherServlet就可以将结果返回给用户了。




