### Data Types
These are the type of values that can be represented and manipulated in a programming language.

The latest ECMAScript standard defines seven data types: six primitive data types and Objects.

### Primitive Data Types 
A primitive data type or value is data that is not an object and has no methods. All primitives are immutable (cannot be changed).

<ul>
  <li>Number: Number represents numerical values. eg. 123, 120.50 etc</li>
  <li>String: JavaScript's String type is used to represent textual data. e.g “Hello”, “name”, “Good morning”;</li>
  <li>Boolean : Boolean represents a logical entity and can have two values: true, and false.</li>
  <li>Null : The Null type has exactly one value: null</li>
  <li>Undefined : A variable that has not been assigned a value has the value undefined.</li>
</ul>

### 
Objects
An object is a collection of properties, and a property is an association between a key and a value. A property's value can be a function, in which case the property is known as a method. 

For example, let's create an object named Student and give it properties named name, school, and age.

```html
<html>
  <body>
    <script type="text/javascript">
      var student = new Object();
      student.name = “Jane”;
      student.school = “TeenCode Academy”;
      student.age = 12;
        
      document.write("<b>”My name is “+ student.name </b>")
      document.write("<b>”I am ” + student.age + “ years old” </b>")
    </script>
  </body>
</html>
```

* The result printed to screen  is as follows:

```
My name is Jane
I am 12 years old
```

Objects can also be defined using **‘{}’**

```html
<html>
  <body>
    <script type="text/javascript">
      var student = {};
      student.name = “Jane”;
      student.school = “TeenCode Academy”;
      student.age = 12;
        
      document.write("<b>”My name is “+ student.name </b>")
      document.write("<b>”I am ” + student.age + “ years old” </b>")
    </script>
  </body>
</html>
```

The result printed to screen  is as follows:

```
My name is Jane
I am 12 years old
```

### Variables
Variables can be thought of as named containers. You can place data into these containers and then refer to the data simply by naming the container.

Variables must be declared before use. Variables are declared with the var keyword as follows.

```javascript
var animal;
var address, age; 
```

You can create a variable and assign a value it later. or assign a value at the time of initialization as follows.

```javascript
var name = ‘John’;
var school;
school = ‘Teencode Academy’;
```

**Note** − Use the var keyword only for declaration or initialization, once for the life of any variable name in a document. You should not re-declare same variable twice. This reassigns the value **Anna** to the **name** variable.

```javascript
var name = ‘John’;
var name = ‘Anna’  X
```

### Variable Names
While naming variables, take note of the following.

<ul>
  <li>Variable names must start with a letter or an underscore character. Numbers 0-9 are not allowed. For example, 3address is an invalid name but _3address is a valid name.</li>
  <li>Variable names are case-sensitive. For example, School and school are two different variables.</li>
  <li>Do not use JavaScript reserved keywords as a variable names. For example, break or boolean are invalid names.</li>
</ul>


### Arrays
The Array object lets you store multiple values in a single variable. It stores a collection of data but it is often more useful to think of an array as a collection of variables of the same type.

You can create array by simply assigning values as follows :

```javascript
var fruits = [ "plum", "guava", "mango", “pawpaw” ];

var scores = [ 20, 50, 100 ];

var values = [“broom”, 20, true]
```

OR using the Array constructor

```javascript
var scores = new Array( 20, 50, 100 );
```

### Array Elements
You will use ordinal numbers to access and to set values(elements) inside an array as follows.

```html
<html>
  <body>
    <script type="text/javascript">
      var fruits = [];

      fruits[0] = “plum”;
      fruits[1] = “guava”;
      fruits[2] = “mango”;
      fruits[3] = “pawpaw”;

      document.write("<b>”Fruits in the array : “+ fruits</b>");
    </script>
  </body>
</html>
```

The result printed to screen  is as follows:
Fruits in the array: plum, guava, mango, pawpaw

### Array Properties
* length: The number of elements int the array can be determined using the length property. Example

```html
<html>
  <body>
    <script type="text/javascript">
      var fruits = [ "plum", "guava", "mango", “pawpaw” ];
      var length = fruits.length;
        
      document.write("<b>’Number of fruits in array: ‘+ length </b>");
    </script>
  </body>
</html>
```

The result printed to screen  is as follows:
Number of fruits array: 4

* constructor: Returns a reference to the array function that created the object.

```html
<html>
  <body>
    <script type="text/javascript">
      var scores = new Array( 20, 50, 100 )
      var scoresConstructor = scores.constructor;
        
      document.write("<b>’Constructor:’ + scoresConstructor  </b>")
    </script>
  </body>
</html>
```

The result printed to screen  is Constructor: [Function: Array]:

* prototype: This property represents the prototype for the Array constructor and allows you to add new properties and methods to all Array objects. Example to add the method to return the first element of the Array:

```javascript
Array.prototype.first = function() {
  return this[0];
}
```

### Array Methods
Some frequently used array methods are:

* concat: this method is used to merge an array to another array or value.

```html
<html>
  <body>
    <script type="text/javascript">
      var breakfast = [‘eggs’, ‘sausages’, ‘tea’];
      var lunch = [‘rice’, ‘potatoes’, ‘beef’];
      var meals = breakfast.concat(lunch);
          
      document.write("<b>Menu for the day :’ + meals </b>");
    </script>
  </body>
</html>
```

The result printed to screen  is 
Menu for the day is ‘eggs’, ‘sausages’, ‘tea’,  ‘rice’, ‘potatoes’, ‘beef’:

* map: Creates a new array with the results of calling a provided function on every element in this array.

```html
<html>
  <body>
    <script type="text/javascript">
      var scores = [1, 5, 10, 15];
      var doubled = scores.map(function(x) {
        return x * 2;
      });
          
      document.write("<b>”Double is now : “ + doubled </b>");
      document.write("<b>”Scores remains : “ + scores </b>");
    </script>
  </body>
</html>
```

The result printed to screen  is 
Doubled is now 2, 10, 20, 30
Scores remains 1, 5, 10, 15

* filter: Creates a new array with all of the elements of this array for which the provided filtering function returns true.

```html
<html>
  <body>
    <script type="text/javascript">
      var vegetables = ["spinach", "cabbage", "lettuce", "cauliflower", "asparagus", "runner-beans"];

      var longVegetables = vegetables.filter(function(vegetable) {
        return vegetable.length > 10;
      });
          
      document.write("<b>”The long vegetables are : “ + longVegetables </b>");
    </script>
  </body>
</html
```

The result printed to screen: 
The long vegetables are  cauliflower, runner-beans

* push: Adds one or more elements to the end of an array and returns the new length of the array.

```html
<html>
  <body>
    <script type="text/javascript">
      var scores = [3, 45, 94];
      scores.push(10);
      document.write("<b>”Scores are now : “ + scores </b>");
    </script>
  </body>
</html>
```

The result printed to screen  is 
Scores are  now : 3, 45, 94, 10

* slice: Extracts a section of an array and returns a new array.

```html
<html>
  <body>
    <script type="text/javascript">
      var numbers = ['zero', 'one', 'two', 'three';
      var sliced = numbers.slice(1, 3);

      document.write("<b>”Numbers: “ + numbers</b>");
      document.write("<b>”Sliced numbers: “ + sliced </b>");
    </script>
  </body>
</html>
```

The result printed to screen  is 
Numbers: zero, one, two, three
Sliced numbers: one, two

* splice: Adds and/or removes elements from an array.

```html
<html>
  <body>
    <script type="text/javascript">
      var dogs = [‘bulldog’, 'chinook', 'barbet', 'beagle'];

      dogs.splice(2, 0, ‘bullmastiff’)); 
      // insert ‘bullmastiff’ at  2-index position

      document.write("<b>”Dog Breeds 1 : “ + dogs</b>");
      dogs.splice(2, 1)); 
      // remove 1 item at 2-index position(‘bullmastiff’)
      document.write("<b>”Dog Breeds 2 : “ + dogs</b>");
    </script>
  </body>
</html>
```

The result printed to screen  is 
Dog Breeds 1: bulldog, chinook, bullmastiff, barbet, beagle
Dog Breeds 2: bulldog, chinook, barbet, beagle

**Note:** [Link to more Array methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
