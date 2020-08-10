1. 作用域对象
* 一个js实例对象，ng-app指令默认会创建一个根作用域对象（$rootScope）
* 它的属性和方法与页面中的指令或表达式关联的
2. 控制器对象
* 用来控制AngularJS应用数据的    实例对象
* ng-controller：指定控制器构造函数，angular会自动new此函数创建控制器对象
* 同时angular还有创建一个新的作用域对象$scope，它是$rootScope的子对象
* 在控制器函数中声明$scope形参（必须是$scope），angular会自动将$scope对象注入

3. new过的对象和自调用的对象区别
* 函数自调用的对象 的this是window
* new过的对象 的this是它的实例对象
