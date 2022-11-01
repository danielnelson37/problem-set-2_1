# Problem Set 2.1
## Types, Values, and Operators

1. What is a _unary operator_? Give an example of one.
An operator that takes one operand. typeOf() is an example of a urnary operator. 

2. What is a _binary operator_? Give an example of one.
An operator that take two values. The + operator is an example of binary operator.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below.
We use the ternary operator to reduce the code of an if-else satement. It takes three operands: a condition followed by a question mark (?), 
then an expression to execute if the condition is truthy followed by a colon (:), and finally the expression to execute if the condition is 
falsy. 

EXAMPLE: 
condition ? exprIfTrue : exprIfFalse


4. What is the difference between using the _strict_ and _non-strict_ equality operators?
The strict equality operator (===) checks whether its two operands are equal, returning a Boolean result. Unlike the equality operator, the 
strict equality operator always considers operands of different types to be different.

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
The seven primitive data types consist of numbers, strings, booleans, null, undefined, and symbol. The last non-primitive data type are objects.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
It'll return string

7. What does the code below return?
  ```javascript
  typeof true;
  ```
It'll return boolean

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
It'll return number

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```
False

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
To be truthy means the value that is considered true in Boolean context. Falsy values are values considered false in Boolean context.
Falsy values consist of 0, -0, NaN, an empty string, undefined, null, and false.

11. Evaluate the following expressions using JavaScripts implicit coercion rules. For each example, in one sentence, explain what coercions were applied and why:
  * `8 * null`
  * `"5" - 1`
  * `"5" + 1`
  * `true + false`
  * `"i am" + undefined`
  * `5 + undefined`


12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
returns false

   ```javascript
   (false || undefined);
   ```
returns false

   ```javascript
   (undefined || false);
   ```
returns false

   ```javascript
   ((false && undefined) || (false || undefined));
   ```

   ```javascript
   ((false || undefined) || (false && undefined));
   ```

   ```javascript
   ((false && undefined) && (false || undefined));
   ```

   ```javascript
   ((false || undefined) && (false && undefined));
   ```

   ```javascript
   ('a' || (false && undefined) || '');
   ```

   ```javascript
   ((false && undefined) || 'a' || '');
   ```

   ```javascript
   ('a' && (false || undefined) && '');
   ```

   ```javascript
   ((false || undefined) && 'a' && '');
   ```

