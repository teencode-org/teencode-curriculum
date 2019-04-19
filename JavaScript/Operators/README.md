### Operators
Let us take a simple expression **4 + 5 is equal to 9**. Here 4 and 5 are called **operands** and ‘+’ is called the **operator**. JavaScript supports the following types of operators.

<ul>
  <li>Arithmetic Operators</li>
  <li>Comparison Operators</li>
  <li>Logical (or Relational) Operators</li>
  <li>Assignment Operators</li>
  <li>Conditional (or ternary) Operators</li>
</ul>

### Arithmetic Operators
Arithmetic operators can be used with numbers in Javascript. Let var a = 30 and var b = 10

* addition(+): adds the two operands a + b equals 40
**Note** - When the + operator is used with a strings and another value, it concatenates them.
>> “Hello” + “world” gives “Hello World”, 10 + “years” gives “10years”;

* subtraction(-) : deducts the second operand from the first. 
>> a - b equals 20

* multiplication(*): multiplies the two operands 
>> a * b equals 300

* division(/): divides the numerator by the denominator.
>> a / b equals 3

* modulus(%): outputs the remainder of an integer division 
>> a % b equals 0

* increment(++): increases an integer value by 1 
>> a++ equals 31

* decrement(--): decreases an integer value by 1. 
>> a-- equals 29

### Comparison Operators
These are used to compare two values. Let var a = 20 and var b = 30.

* equal(= =): checks if the value of two operands are equal or not, if yes, then the condition becomes true.
>> (a == b) is not true

* not equal(! =): checks if the value of two operands are equal or not, if the values are not equal, then the condition becomes true.
>> (a != b) is true

* greater than(>): checks if the value of the left operand is greater than the value of the right operand, if yes, then the condition becomes true. 
>> (a > b) is not true.

* less than(<): checks if the value of the left operand is less than the value of the right operand, if yes, then the condition becomes true. 
>> (a < b) is true

* greater than or equal to(>=): Checks if the value of the left operand is greater than or equal to the value of the right operand, if yes, then the condition becomes true.
>> (a >= b) is not true.

* less than or equal to(>=): Checks if the value of the left operand is less than the value of the right operand, if yes, then the condition becomes true. 
>> (a < b) is true


### Logical Operators
Let var a = 20 and var b = 30

* AND(&&): If both the operands are non-zero, then the condition becomes true. 
>> (a && b) is not true

* OR(||): If any of the two operands are non-zero, then the condition becomes true.
>> (a || b) is true

* NOT(!): Reverses the logical state of its operand. If a condition is true, then the Logical NOT operator will make it false. 
>> !(a && b) is false.


### Assignment Operators
* simple Assignment(=): Assigns values from the right side operand to the left side operand

```html
<html>
  <body>
    <script type="text/javascript">
      var a = 20, b = 30;
      var c = a + b;

      document.write("<b>”Result ” + c </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result 50

* add and assignment(+=) : adds the right operand to the left operand and assigns the result to the left operand.

```html
<html>
  <body>
    <script type="text/javascript">
      var d = 0, a = 30;
      d += a;
      // this is equivalent to d = d + a

      document.write("<b>”Result ” + d </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result 30

* subtract and assignment(-=): It subtracts the right operand from the left operand and assigns the result to the left operand.

```html
<html>
  <body>
    <script type="text/javascript">
      var d = 20, a = 10;
      d -= a;
      // this is equivalent to d = d - a

      document.write("<b>”Result ” + d </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result 10

* divide and assignment(/=): It divides the left operand with the right operand and assigns the result to the left operand.

```html
<html>
  <body>
    <script type="text/javascript">
      var d = 20, a = 10;
      d /= a;
      // this is equivalent to d = d / a

      document.write("<b>”Result ” + d </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result 2

* multiply and assignment(*=): It multiplies the right operand with the left operand and assigns the result to the left operand

```html
<html>
  <body>
    <script type="text/javascript">
      var d = 20, a = 10;
      d *= a;
      // this is equivalent to d = d * a

      document.write("<b>”Result ” + d </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result 200

* modulus and assignment(%=): It takes modulus using two operands and assigns the result to the left operand.

```html
<html>
  <body>
    <script type="text/javascript">
      var d = 20, a = 10;
      d %= a;
      // this is equivalent to d = d % a

      document.write("<b>”Result ” + d </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result 0


### Conditional Operator (? :)
The conditional operator first evaluates an expression for a true or false value and then executes one of the two given statements depending upon the result of the evaluation. 

```html
<html>
  <body>
    <script type="text/javascript">
      var d = 10;
      var e = d == 10 ? true : false;
      // If Condition is true? Then e = true : else e = false 

      document.write("<b>”Result ” + e </b>");
    </script>
  </body>
</html>
```

The output printed to screen is:
Result true


### typeof Operator
The **typeof** operator is used to determine the data type of an operand. Its evaluates to a string indicating the data type.

Below are the return values for the **typeof** Operator:

| Type  | String Returned by typeof |
| ---   | ---                       |
| String  | “string”                |
| Number  | “number”                |
| Boolean | “boolean”               |
| Function  | “function”            |
| Object    | “object”              |
| Undefined | “undefined”           |
| Null      | “object”              |


### Example

```html
<html>
  <body>
    <script type="text/javascript">
      var result;
      var age = 20;
      var name = “Donald”
        
      result = typeof age;
      document.write("<b>”Age is just a ” + result </b>");

      result = typeof name;
      document.write("<b>”My name of data type ” + result </b>");
    </script>
  </body>
</html>
```

The output is as follows:
Age is just a number
My name is of data type string
