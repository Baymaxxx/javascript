var array = [1,6,3];

var array = [
	163,
	"netease",
	{color:"red"},
	[],
	true
];

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.length;  // 3
students = [];
students.length;  // 0

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students[0];        // {id:1,score:80}
students[0].score;  // 80
students[1].score = 60;

var telephones = [110,120,114];
telephones.indexOf(120);  // 1
telephones.indexOf(119);  // -1

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
var editScore = function(item,index,array){
	item.score += 5;
};
students.forEach(editScore);

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.reverse();
students[0].score;  // 70

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
var byScore = function(a,b){
	return b.score-a.score;
};
students.sort(byScore);

var studentNames = ["wq","xl","gp"];
studentNames.sort();
studentNames;  // ["gp","wq","xl"]

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.push({id:4,score:90});

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.push({id:4,score:90},{id:5,score:60});

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.unshift({id:4,score:90});

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.shift();  // {id:1,score:80}

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.pop();  // {id:3,score:70}

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.splice(1,1,{id:4,score:90});

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.splice(1,1);

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
students.splice(1,0,{id:4,score:90});

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
var newStudents = students.slice(0,2);

var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
var newStudents = students.slice(0);

var students1 = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
var students2 = [
	{id:4,score:90},
	{id:5,score:60}
];
var students3 = [
	{id:6,score:40},
	{id:7,score:30}
];
var newStudents = students1.concat(students2,students3);

var emails = ["wq@163.com","gp@163.com","xl@163.com"];
emails.join(";");  // "wq@163.com;gp@163.com;xl@163.com"

var scores = [60,70,80,90];
var newScores = [];
var addScore = function(item,index,array){
	newScores.push(item+5);
};
scores.forEach(addScore);
newScores; // [65,75,85,95]

var scores = [60,70,80,90];
var addScore = function(item,index,array){
	return item+5;
};
scores.map(addScore);  // [65,75,85,95]


var students = [
	{id:1,score:80},
	{id:2,score:50},
	{id:3,score:70}
];
var sum = function(previousResult,item,index,array){
	return previousResult+item.score;
};
students.reduce(sum,0);  // 200
