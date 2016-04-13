var car = {
	color : "red",
	run : function(){alert("run")}
};
car.color;     // "red"
car.run();     // alert("run")
car["color"];  // "red"
car["run"]();  // alert("run")

var car = {
	color : "red",
	run : function(){alert("run")}
};
car.type = "suv";
car.stop = function(){alert("stop")};

var car = {
	color : "red",
	run : function(){alert("run")}
};
car.color = "white";
car.run = function(){alert("run2")};

var car = {
	color : "red",
	run : function(){alert("run")}
};
delete car.color;
car.color;  // undefined

var car = {
	color : "red",
	run : function(){alert("run")}
};
car.constructor;   // Object

var num = new Number(123);
num.constructor;   // Number

var num = new Number(123);
num.toString();  // "123"

var num = new Number(123);
num.valueOf();   // 123

var car = {
	color : "red",
	run : function(){alert("run")}
};
car.hasOwnProperty("color");  // true
car.hasOwnProperty("logo");   // false