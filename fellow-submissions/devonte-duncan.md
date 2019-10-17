# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.

  A unary operator like any operator performs an operation on some argument or operand. One example is the ++ operator which adds one to its operand.

2. What is a _binary operator_? Give an example of one.

  A binary operator AKA boolean operator is an operator that determines the binary value of the operand. One example is the "!"( not operator), which returns the opposite binary value of the operand's default value.  

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?

  We use a ternary operator as a shorthand for simple if else statements. Here's an example:
  
  let falseByDefault = true;
  falseByDefault ? console.log('This is what this code alone would output.') : console.log('This code would not run as the variable declare is abstractly equal to the binary value of true.');

4. What is the difference between using the _strict_ and _non-strict_ equality operators?

  The strict equality operator '(===)', compares its two operands to see if they're equal in type and in content. Meanwhile the non-strict equality operator '(==)', coerces both operands to be the same type then compares to see if they're equal in content.

5. What are the seven JavaScript data types? Which of these are considered _primitive_?

  The seven JavaScript data types are:
   - strings //Primative
   - numbers  //Primative
   - null  //Primative
   - undefined  //Primative
   - boolean  //Primative
   - symbols // Primative
   - objects

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
  This code will return 'string'.

7. What does the code below return?
  ```javascript
  typeof true;
  ```
  This code will return 'boolean'.

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
  This code will return 'number'.

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
   This code will return 'object'. This is because null is considered an object devoid of data by javascript.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

   Truthy and falsy are the inherent boolean values of things in JavaScript. A truthy type is inherently true. While a falsy type is inherently false.
   
   Here are the six falsy values:
   - null
   - '' (empty string)
   - undefined
   - 0
   - NaN
   - false
   

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:

  * `8 * null` = 0  [null is coerced to be 0 because the rule is when an arithmetic operator is used both operands will be coerced to be numbers.]
  * `"5" - 1` = 1 [5 is coerced to be 0 because the rule is when an arithmetic operator is used both operands will be coerced to be numbers.]
  * `"5" + 1` = 4 [5 is coerced to be 0 because the rule is when an arithmetic operator is used both operands will be coerced to be numbers.]
  * `true + false` = 1 [True is coerced to be 1 and False is coerced to be 0 because the rule is when an arithmetic operator is used both operands will be coerced to be numbers.]
  * `"i am" + undefined` = i amundefined [i am is a string that isn't abstractly a number so "undefined" is coerced into being a string.]
  * `5 + undefined` = NaN [undefined has no numerable value and 5 is number, so naturally the addition of these two things is not a number (NaN).]

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
   false

   ```javascript
   (false || undefined);
   ```
    undefined

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
    undefined
    
   ```javascript
   ((false || undefined) || (false && undefined));
   ```
    undefined

   ```javascript
   ((false && undefined) && (false || undefined));
   ```
    false
   
   ```javascript
   ((false || undefined) && (false && undefined));
   ```
    false
   
   ```javascript
   ('a' || (false && undefined) || '');
   ```
    'a'
   
   ```javascript
   ((false && undefined) || 'a' || '');
   ```
     'a'
     
   ```javascript
   ('a' && (false || undefined) && '');
   ```
     undefined

   ```javascript
   ((false || undefined) && 'a' && '');
   ```
     undefined