"# lecture-6" 
# What is a object in java script ?
# JavaScript Objects
## In the JavaScript data types tutorial, you learned about 7 different primitive data types. And here, you are going to learn about the eighth data-type (JavaScript object).

 ### JavaScript object is a non-primitive data-type that allows you to store multiple collections of data.


 ###  Note: If you are familiar with other programming languages, JavaScript objects are a bit different. You do not need to create classes in order to create objects.

 ### Here is an example of a JavaScript object.

// object
const student = {
    firstName: 'ram',
    class: 10
};
  ### Here, student is an object that stores values such as strings and numbers.

 ### JavaScript Object Declaration
 ### The syntax to declare an object is:

const object_name = {
   key1: value1,
   key2: value2
}
 ### Here, an object object_name is defined. Each member of an object is a key: value pair separated by commas and enclosed in curly braces {}.

 ###  For example,

// object creation
const person = { 
    name: 'John',
    age: 20
};
console.log(typeof person); // object
Run Code
You can also define an object in a single line.

const person = { name: 'John', age: 20 };
In the above example, name and age are keys, and John and 20 are values respectively.

  ![Alt-текст](Screenshot%202023-11-30%20164400.png/ "Заголовок изображения") 

There are other ways to declare an object in JavaScript. To learn more, visit Different Ways to Declare JavaScript Objects.

JavaScript Object Properties
In JavaScript, "key: value" pairs are called properties. For example,

let person = { 
    name: 'John',
    age: 20
};
Here, name: 'John' and age: 20 are properties.

Example of JavaScript object properties
JavaScript object properties
Accessing Object Properties
You can access the value of a property by using its key.

# 1. Using dot Notation
Here's the syntax of the dot notation.

objectName.key
For example,

const person = { 
    name: 'John', 
    age: 20, 
};

// accessing property
console.log(person.name); // John
Run Code
# 2. Using bracket Notation
Here is the syntax of the bracket notation.

objectName["propertyName"]
For example,

const person = { 
    name: 'John', 
    age: 20, 
};

// accessing property
console.log(person["name"]); // John
Run Code
JavaScript Nested Objects
An object can also contain another object. For example,

// nested object
const student = { 
    name: 'John', 
    age: 20,
    marks: {
        science: 70,
        math: 75
    }
}

// accessing property of student object
console.log(student.marks); // {science: 70, math: 75}

// accessing property of marks object
console.log(student.marks.science); // 70
Run Code
In the above example, an object student contains an object value in the marks property.

  ### JavaScript Object Methods
In JavaScript, an object can also contain a function. For example,

const person = {
    name: 'Sam',
    age: 30,
    // using function as a value
    greet: function() { console.log('hello') }
}

person.greet(); // hello



# Methods object

## Методҳои объектӣ дар JavaScript метавонанд бо истифода аз функсияҳо дастрас шаванд. Функсияҳо дар JavaScript ҳамчун арзишҳои амвол нигоҳ дошта мешаванд. Объектҳоро инчунин бидуни истифодаи қавс () даъват кардан мумкин аст. 

##  Дар як усул, "ин" ба объекти соҳиб ишора мекунад.
## Маълумоти иловагиро инчунин дар баробари усули объект илова кардан мумкин аст.
# Синтаксис: 

## objectName.methodName()
## Хусусиятҳо: Функсияро ба арзишҳои амволӣ тақсим кардан мумкин аст, ки баъдан якҷоя карда мешаванд ва якҷоя баргардонида мешаванд. 
Масалан: Функсияи донишҷӯ дорои хосиятҳои зерин мебошад: 

ном
синф
ҷудокунӣ
Арзиши бозгашт: Он усулҳо/функсияҳоеро, ки ҳамчун хосиятҳои объект нигоҳ дошта мешаванд, бармегардонад.


function getObjectLength() {

	// Declare an object
	exampleObject = {
		id: 1,
		name: 'Arun',
		age: 30
	}

	// Using Object.keys() method to get length
	objectLength = Object.keys(exampleObject).length;
	console.log(objectLength);
}
getObjectLength();


# Усули Object.entries()статикӣ массиви ҷуфтҳои калиди-арзиши моликияти шуморашавандаи дорои сатри калиддори объекти додашударо бармегардонад.

# Объект.калидҳо, арзишҳо, вурудот
 ##  Биёед аз сохторҳои инфиродии додаҳо дур шавем ва дар бораи такрори онҳо сӯҳбат кунем.

##  Дар боби гузашта мо усулхои map.keys(), map.values(), map.entries().

# Ин усулҳо умумӣ мебошанд, барои истифодаи онҳо барои сохторҳои додаҳо як созишномаи умумӣ вуҷуд дорад. Агар мо ягон вақт сохтори додаҳои худро эҷод кунем, мо бояд онҳоро низ татбиқ кунем.

Онҳо барои:

Map
Set
Array
# Объектҳои оддӣ низ усулҳои шабеҳро дастгирӣ мекунанд, аммо синтаксис каме фарқ мекунад.

# bОбъект.калидҳо, арзишҳо, вурудот
Барои объектҳои оддӣ, усулҳои зерин мавҷуданд:

Object.keys(obj) – массиви калидҳоро бармегардонад.
Object.values(obj) – массиви арзишҳоро бармегардонад.
Object.entries(obj) – массиви [key, value]ҷуфтҳоро бармегардонад.
Лутфан фарқиятҳоро қайд кунед (масалан, дар муқоиса бо харита):
![Alt-текст](Screenshot%202023-11-30%20165608.png/ "Заголовок изображения")