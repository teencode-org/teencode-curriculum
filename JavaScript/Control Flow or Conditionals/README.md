### Control Flow or Conditionals
There may be situations in a program that you need to make decisions about what happens based on some conditions. JavaScript supports conditional statements which are used to perform different actions based on different conditions. Examples are:

### if..else statements
JavaScript supports the following forms of **if..else** statement:

<ul>
  <li>if statement</li>
  <li>if...else statement</li>
  <li>if...else if... statement.</li>
</ul>

### if statement
The **if** statement executes the statement only if the conditions is true or if the test  expression evaluates to true. If the condition evaluates to false, then no statement would be not executed.

**Syntax**

```javascript
if (condition or expression) {
   code block be executed if condition evaluates to true
}
```

Example:
Case 1:

```html
<html>
  <body>
    <script type="text/javascript">
      var age = 20;
      
      if( age >= 18 ) {
        document.write("<b>Qualifies for driving</b>");
      }
    </script>
  </body>
</html>
```

In **Case 1** ‘Qualifies for driving’ will be printed to screen as 20 is greater than 18’

Case 2:

```html
<html>
  <body>
    <script type="text/javascript">
      var age = 12;
      
      if( age < 18 ) {
        document.write("<b>Does not qualify for driving</b>");
      }

    </script>
  </body>
</html>
```

In **Case 2** ‘Does not qualify for driving’ will not be printed to screen as 12 is less than 18’


### if...else statement:
The **if...else** statement executes the first statement only if the conditions is true or if the test expression evaluates to true. If the condition evaluates to false, then next statement would be executed.

**Syntax**

```javascript
if (condition or test expression) {
	code block be executed if condition evaluates to true
} else {
  code block be executed if condition evaluates to false
}
```

Example

```html
<html>
  <body>
    <script type="text/javascript">
      var age = 20;
      
      if ( age >= 18 ) {
        document.write("<b>Qualifies for driving</b>");
      } else {
        document.write("<b>Does not qualify for driving</b>");
      }
    </script>
  </body>
</html>
```

In this example, ‘Qualifies for driving’ will be printed to screen as 20 is greater than 18’

### if...else if... statement
The **if...else if...** allows the program to make a correct decision out of several conditions. Statement(s) are executed based on the true condition, if none of the conditions is true, then the **else** block is executed.

**Syntax**
The syntax of an if-else-if statement is as follows:

```javascript
if (condition1) {
	code block be executed if condition1 evaluates to true
} else if (condition2) {
  code block be executed if condition2 evaluates to true
} else if (condition3) {
  code block be executed if condition3 evaluates to true
} else {
  code block be executed if all conditions evaluates to false
}
```

Statement(s) are executed based on the true condition, if none of the conditions is true, then the **else** block is executed.


Example

```html
<html>
  <body>
    <script type="text/javascript">
      var age = “unknown;
      
      if( age >= 18 ) {
        document.write("<b>Qualifies for driving</b>");
      } else if(age < 18) {
        document.write("<b>Does not qualify for driving</b>");
      }  else {
        document.write("<b>Age is not a number!</b>");
      }
    </script>
  </body>
</html>
```

In this example, ‘Age is not a number|’ will be printed to screen as ‘unknown’ is not a number


### Switch Statement 
The switch statement evaluates an expression, matching the expression's value to a case clause, and executes statements associated with that case.  If nothing matches, a default condition will be used.

**Syntax**
```javascript
switch (expression) {
  case condition 1: 
    statement(s)
    break;

  case condition 2: 
    statement(s)
    break;
  .
  .
  .
  
  case condition n: statement(s)
    break;
  
  default: 
    statement(s)
}
```


The break statements indicate the end of a particular case. If they were omitted, the interpreter would continue executing each statement in each of the following cases.

Example
Try the following example to implement switch-case statement.

```html
<html>
  <body>
    <script type="text/javascript">
      
      var status='done';

      switch (status) {
        case 'ready':
          document.write("Getting Ready<br />");
          break;
      
        case 'started':
          document.write("Started program<br />");
          break;
      
        case 'progress':
          document.write("Work in progress<br />");
          break;
      
        case done:
          document.write("All Set and ready to go<br />");
          break;
      
        default: 
          document.write("Unknown status<br />")
      }  
    </script>
  </body>
</html>
```

In this example, ‘All set and ready to go’ will be printed to screen as status equals done’


### The while Loop
The while loop executes a code block repeatedly as long as an expression or test condition is true. Once the expression becomes false, the loop terminates. The condition is evaluated every time before executing the statement.

**Syntax**

```javascript
while (expression){
  code block to be executed if expression evaluates to true
}
```

Example
```html
<html>
  <body>
    <script type="text/javascript">
      var counter = 0;
      document.write("while loop starts here");
      while (counter < 5) {
        document.write("Current count is " + counter +  "<br />");                      
        counter++;
      }

      document.write("while loop ends here");
    </script>
  </body>
</html>
```

In this example, the following results are printed to screen:

```javascript
while loop starts here
Current count is 0
Current count is 1
Current count is 2
Current count is 3
Current count is 4
while loop ends here
```

### The do...while Loop
The do...while loop executes a specified statement until the test statement or condition evaluates to false. The condition check happens after the loop has run at least once.

**Syntax**

```javascript
do {
  code block to be executed;
}
```

```html
<html>
  <body>
    <script type="text/javascript">
      var counter = 0;
      document.write("While loop starts here");
      do {
        document.write("Current count is " + counter +  "<br />");                      
        counter++;
      }
      while(counter < 5);

      document.write("do while loop ends here");
    </script>
  </body>
</html>
```

In this example, the following results are printed to screen:

```javascript
do while loop starts here
Current count is 0
Current count is 1
Current count is 2
Current count is 3
Current count is 4
do while loop ends here
```

### FOR LOOP
A for loop is declared with an initialization, test statement and final expression. The loop is executes a block of code or statements for the number of the test statement evaluates to true

- The **initialization**: the counter to a starting value at the start of the loop.
- The **test statement**: this will test if a given condition is true or not. If the condition is true, then the code given inside the loop will be executed, otherwise the control will come out of the loop.
- The **final expression** This evaluates at the end of each loop iteration before the next evaluation of condition. This is mostly used to increment or decrement a counter.

**Syntax**

```javascript
for (initialization; test condition; final expression){
  Statement(s) to be executed if test condition is true
}
```

Example

```html
<html>
  <body>
    <script type="text/javascript">
      var counter;
        document.write("for loop starts here");
        for (counter = 0; counter <= 5; counter++){
        document.write("Current count is " + counter +  "<br />");                      
      }
      while(counter < 5);

      document.write("for loop ends here");
    </script>
  </body>
</html>
```

In this example, the following results are printed to screen:

```javascript
for loop starts here
Current count is 0
Current count is 1
Current count is 2
Current count is 3
Current count is 4
Current count is 5
for loop ends here
```
