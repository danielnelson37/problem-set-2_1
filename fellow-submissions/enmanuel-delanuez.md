# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
    - A unary operator performs an action to a single operand. An example of a unary operator is the `! : logical NOT operator`. It can be used like so: `!true === false`

2. What is a _binary operator_? Give an example of one.
    - A binary operator functions with two operands. Binary operators include *arithmatic operators* and *equality operators*, because while their function may differ they take two operads like so: `15 % 4`.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
    - The ternary operator takes three operands. Ternary operators is used to simplify *if...else* statements like so:
    `let isCorrect = true;
     isCorrect ?
     console.log('Correct!'):
     console.log('Incorrect!');`
This code snippet declares a variable with the boolean value `true`. The ternary operator `?` takes the first operand `isCorrect` preceeding it and determines whether it is or *truthy* or *falsy*. If truthy, the operand to following it will be executed. Else, the operand following `:` will be executed.

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
    -

5. What are the seven JavaScript data types? Which of these are considered _primitive_?

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```

7. What does the code below return?
  ```javascript
  typeof true;
  ```

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
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

   ```javascript
   (false || undefined);
   ```

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
