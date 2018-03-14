-------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------

 /* global console, alert, prompt, document */
 /* jsLint pluspluse: true */

-------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------

  Get && Set
  ----------------------

-------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------

| Where Put The JavaScript Code |
---------------------------------

 => inline => HTML attribute onclick = "function name()"

  <script>
 => internal => document.write(" ----- ");
  </script>

 => external => <script src="JavaScript/Plugins.js"></script>

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Syentax |
-----------

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Variable |
------------

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Data Type |
-------------

 => => number
 => => string
 => => array
 => => bolian
 => = " " => null
 => undefined => undefined
 => => object

 // typeOf();

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| OutPut |
----------

 => document.write(" ----- ");
 => alert (" ----- ");
 => console.log (" ----- ");
 => inner HTML = ;

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| InPut |
---------

 => prompt("text", "example value");

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Operators |
-------------

 =>( < ) => greater than
 =>( > ) => esser than
 =>( = ) => assignment operator

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

|( Conditional || comparision ) Operators |
-------------------------------------------

 =>( <= ) =>
 =>( >= ) =>
 =>( == ) => comparision operator => compare " value "
 =>( === ) => identical operator => compare " value " + " data type "

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Logical Operators |
---------------------

 =>( ! ) => not
 =>( != ) => not equal
 =>( !== ) => not identical => not equal in " value " + " data type "
 =>( === ) => identical operator
 =>( && ) => and
 =>( || ) => or

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| If Cases |
------------

 => if(condition) {

  statements;

  } else if(condition) {

  statements;

  } else if(condition) {

  statements;

  } else(condition) {

  statements;

  }

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Loop |
--------

Syntax
------

 => for(initialization; condition; final expression) {
  statements;
  }
EX
--

  var i;
 => for(i = 0; i < 10; i++) {
  console.log(i);
  }

-------------------------------------------------------------------------------------------------------

 => while(condition) {
  statements;
  final expression
  }

EX
--

  var i;
 => while(i < 10) {
  console.log(i);
  i++
  }

-------------------------------------------------------------------------------------------------------

 => do {
  statements;
  final expression
  } while(condition);

EX
--

  var i;
 => do {
  console.log(i);
  i++
  } while(i < 10);

-------------------------------------------------------------------------------------------------------

// Loop Controler :
  => break; =>
  => continue; =>

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Function |
------------

=> function -----(parameter1, parameter2, parameter3, ..... ) {

  "use strict";

  statements;

  retern -----;

  };

//( invoke || call ) function :
  => create a botton with html atribbute => onclick = "function name()"
  => in javascript => function name();

// Sef Invoke Function :
  =>(function -----(parameter1, parameter2, parameter3, ..... ) {
  statements;
  retern -----;
  }())

// "what happen in function stay in function"

// Types of Function :
  => Built-in => " ready to use "
  => Custom Fanction => " which you defined it "

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Events |
----------

Write Event By All Methods :
----------------------------

  <div id="te">sabry ALzahar</div>
  <button id="btn" onclick="change()" > change color </button>

-------------------------------------------------------------------------------------------------------

=> function change() {
  "use strict";
  document.getElementById('te').style.color = "red";
  }

-------------------------------------------------------------------------------------------------------
=> document.getElementById('btn').onclick = function() {
  "use strict";
  te.style.color = "red";
  }

-------------------------------------------------------------------------------------------------------

=> function change() {
  "use strict";
  document.getElementById('te').style.color = "red";
  }
  document.getElementById('btn').onclick = change;

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 addEventListener("eventHandler", function);
 removeEventListener("eventHandler", function);
 Event -driven programming
Event handler = event listener -> الدوال التي تعمل عندما يحدث

DOM Level 0 events API

<input type="button" value='اضغط هنا' onClick="alert('تم الضغط')">

DOM Level 2 events API
-------------------------------------------------------------------------------------------------------

| Switch |
----------

EX :
----

var season = prompt("what is the best season for you ?");

switch(season)

case "winter":
alert("winter is too cold");
break;

case "summer":
alert("summer is too cold");
break;

case "autumn":
case "spring":
alert("this season is amazing");
break;

default:
alert("you didn't enter a season name");
break;

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Array |
---------

Litral Way
----------
=> var friends = ["sabry", "ahmed", "mostafa", "omar", "yasser"];

=> var friends = [
  "sabry",
  "ahmed",
  "mostafa",
  "omar",
  "yasser"
  ];

=> var friends = [];
  friends [0] = "sabry",
  friends [1] = "ahmed",
  friends [2] = "mostafa",
  friends [3] = "omar",
  friends [4] = "yasser";

Constractor Way
----------------

=> var friends = new array("sabry", "ahmed", "mostafa", "omar", "yasser");

=> var friends = new array();
  friends [0] = "sabry";
  friends [1] = "ahmed";
  friends [2] = "mostafa";
  friends [3] = "omar";
  friends [4] = "yasser";

=> var friends = new array(
  "sabry",
  "ahmed",
  "mostafa",
  "omar",
  "yasser"
  );

// " array is zero based index "

// element 1 => index 0
  element 3 => index 2
  element 5 => index 4

// array check :
  =>if(array.isArray(friend)) {
  console.log("good this is array");
  } else {
  console.log("no this isn't array");
  }
// length : var dem = "java script";

  consoe.log(dem.length); =>11 digits = strings + spaces
// array get length :
  console.log(friends.length); => number of array elements

// array set length :
  length = 2; => 1 && 2 element only
  console.log(friends) => ["sabry", "ahmed"]

// convert array to string :
  console.log(friends.toString());
  ||
  console.log(friends.toLocalString());
  ||
  console.log(friends.join(" - ")); || console.log(friends.join(" , "));
// add elements :
  => length => firends[length] = "sayed";
- in last => push(); => firends.push("ali", "khaled", "ramadan",.... );
- in first => unshift(); => firends.unshift("ali", "khaled", "ramadan",.... );
- by index => splice(); => firends.splice(index, how many remove, add item 1, add item 2, ...);

// remove elements :
  => length => firends[length] = "sayed";
- in last => pop(); => firends.pop("ali", "khaled", "ramadan",.... );
- in first => shift(); => firends.shift("ali", "khaled", "ramadan",.... );
- by index => splice(); => firends.splice(index, how many remove, add item 1, add item 2, ...);

// array reverse => index [last] to index [0] => firends.reverse(); console.log(friends);

// array sort => A to Z => firends.sort(); console.log(friends);
// array sort => Z to A => firends.sort(); firends.reverse(); console.log(friends);

// array slice => => var x = firends.slice(start, end); console.log(x);

// array concatenation => firends + array 2 + array 3 => var all = firends.concat(array 2, array 3);

// array search => top to bottom => firends.indexOf("yasser", start index);
// array search => bottom to top => firends.lastIndexOf("yasser", start index);

// print first element in array => console.log(firend.shift());

// print last element in array => console.log(firend.pop());

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Strings Methods |
-------------------

  var x = "i love javascript and json"

=> toString();
=> indexOf(value, start postion-d=0);
=> lastIndexOf(value, end postion-d=0);
=> search();

=> split(separetor, limt);
  -> x.split(" ", 3); => ["i" , "love" , "javascript"]
  -> x.split("a", ); => ["i love j" , "v" , "script" , "nd json"]
=> slice(start , end); => +,-
=> subStr(start , length);
=> subString(start , end);

=> charAt("index"); => x.charAt(5); => "e"
=> charCodeAt("index"); => x.charCodeAt(5); => e => 76
=> replace(value, new value); => x.replace(/javascript/gi, "php") => "i love php and json"

=> String.fromCharCode(115, 97, 98, 114, 121); => sabry
=> .concat(,,,,...);

=> .repeat(repeat number);
=> .tolowerCase();
=> .toUpperCase();

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Object |
----------
 => var myCar = {
  color: red,
  type: via,
  price: 50.000,
  module: 2017
 };
 console.log(myCar.type);

Dynamic Object = Hash Table

Get :-

 - object.prppertyName   -> dot notation
 - object[prppertyName]  -> supscript notation

Set :-

 - object.prppertyName  = 
 - object[prppertyName] = 

Delete :-

 - delete object.prppertyName
 - delete object[prppertyName]


identifier    [variable, function, class, [object, property]] name
------------
-  characters
-  numbers
-  _  -> Machines
-  $  -> Browsers


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Math |
--------

 => Math.ceil();
 => Math.floor();
 => Math.round();
 => Math.min();
 => Math.max();
 => Math.random(); => from 0 to 1
 => Math.pow(x,y); => x^y
 => Math.sqrt(); => root
 => Math.abs(); => abslute value

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Regular Expression | used with : [ search | replace | match | split | test ]
----------------------
  /pattern/attribute

  attributes list

=> [g] => global search
=> [i] => insensitive case
=> [m] => multi line search

  =>
  =>
  =>
  =>

// without double qoutes

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Date |
--------

 => new Date("");

 // Date Format :
  => full format => new Date("");
  => long format => new Date("");
  => short format => new Date("M/D/Y HH:MM:DD");
  => ISO format => new Date("YYYY-MM-DD HH:MM:SS TZD"); => # used #

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
| Incrment & discrment |
------------------------

i++ => i = i + 1
i-- => i = i - 1
i += x => i = i + x
i -= x => i = i - x
i *= x => i = i * x
i /= x => i = i / x
i %= x => i = i % x

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Window Method |
-----------------

 => window.#anything
 => /n
 => prompt("text", "example value");
 => alert();
 => confirm(); => boolean value(true , false )
 => setTimeOut(function, milesecond, param1, param2, ......);
 => clearTimeOut(myTime);
 => var myInterval = setInterval(function, milesecond, param1, param2, ......);
 => clearSetInterval(myInterval);
 => window.open(url, target, spacification, history replace);
 => scrollBy(x, y); => =,-
 => scrollTo(x, y); => =,-
 => stop();
 => .close();
 => .foucus();

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Window Proprites |
--------------------

=> .innerHeight();
=> .innerWidth();
=> .outterHeight();
=> .outterWidth();

=> .scrollx(); = .pageXOfset();
=> .scrolly(); = .pageYOfset();

=> .location.href = "http://www.";

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| |
-----------------------

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| |
-----------------------

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Find Elements by Id , Calss , Tag |
-------------------------------------

 => document.getElementById('...');
 => document.getElementsByTagName('...');
 => document.getElementsByClassName('...');
 => document.quarySelectorAll('...');
 => document.quarySelector('...');

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Colactions
| Find Elements by Object |
---------------------------

 => document.title
 => document.body
 => document.images
 => document.forms
 => document.links
 => document.anchors

 # like array but have no methods expect .length

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| GET & SET Element Content |
-----------------------------

=> innerHTML => text + html
=> outterHTML => text + html
=> textContent => text only

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| GET & SET Attribute Value |
-----------------------------

=> Eement.attribute; || getAttribure(attribute name,);
=> Eement.attribute = "...."; || setAttribure(attribute name, value);
=> hasAttribure(attribute name);
=> removeAttribure(attribute name);

// class attribute => className

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Class List |
--------------

=> .classList();
=> .classList.lenght;
=> .classList.contains('class1', 'class2', .....);
=> .classList.items(class index);
=> .classList.add('class1', 'class2', .....); || .classList += "'class1', 'class2', .....";
=> .classList.remove('class1', 'class2', .....); || .classList -= "'class1', 'class2', .....";
=> .classList.toggle('class1', 'class2', .....);

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
| Child | child = "HTML tags only"
---------

=> .children;
=> .children(child index);
=> .children.length; || .childElementCount;
=> .firstElementChild;
=> .lastElementChild;

=> .appendChild();
=> .createElement();
=> .createTextNode();
=> .createComment();

// create attribute

.createAttribute(/*attributeName*/);
/*attributeName*/.value = " ";
/*element*/.setAttributeNode(/*attributeName*/);

EX :
----

var myMainDiv = document.getElementById('main'),

  // create div element

  myNewEement = document.createElement('div'),

  // create p element

  myNewP = document.createElement('p'),

  // create text node

  myText = document.createTextNode("hello from javascript");

// append text to the new element

myNewEement.appendChild(myText);

// append the new element to my main div

myMainDiv.appendChild(myNewEement);

// append my new p to my main div

myMainDiv.appendChild(myNewP);

=> .insertBefore(element, place);

=> .removeChild(child name);

=> .tagName;

=> .parantElement; = .parantNode;

=> .nextElementSibiling;
=> .previousElementSibiling;

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Node | Node = "HTML tags" + "artributes" + "comments" + "space / text"
--------

=> .childNodes;
=> .childNodes(child index);
=> .childNodes.length;
=> .firstChild;
=> .lasttChild;

=> .nodeName;
=> .nodeName;

=> .cloneNode(false || true);

=> .nextSibiling;

=> .previousSibiling;

// .cloneNode(); = .cloneNode(false);
// .cloneNode(); => clone tag and his attributes without his content (text)
// .cloneNode(false); => clone tag && his attributes without his content (text)
// .cloneNode(true); => clone tag && his attributes && his content (text)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Callback Function |
---------------------

=> setTimeOut(function, milliseconds, param1, param2, ...);
=> setInterval(function, milliseconds, param1, param2, ...);

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| |
-----------------------
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 => document.getElementById("test").innerHTML; => <div>
 => document.getElementById("test").value; => <input>
 => XOR

 => var doc = "hi /"sabry/""; => hi "sabry"
 => var doc = 'hi "sabry"'; => hi "sabry"

 => .focus;
 => .blur;

 => .style.properity = "value";

 => this.
 => document.inputEncoding;
 => document.lastModified;
 => document.URL;

 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| ES6 |
-----------------------


| Destructing |
-----------------------
var info ={
            "id":1,
            "name":"sabry",
            "age":19,
          };


var {id,name,age} = info;
var {id,name:fullName,age} = info;



| swaping |
------------

let a=5,
    b=10;

> [a,b]=[b,a];

> let temp;
  temp = a;
  a=b;
  b=temp;


Template String


var req = new XMLHttpRequest();
req.open("get", "http://randomuser.me/api/?results=10");
req.response();
req.send();
req.status();
req.onload();

JSON.parse();

var Error = new Error();

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Design Pattern |
-------------------
improved virsion from chainnig assingment
function foo() {
var a, b;

// 
a = b = 0; // both local

}





* single var declaration pattern :


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

| Arrow Function |
-------------------

function fun (num) {
  return num * num;
}



var fun = (num) -> num * num;





















