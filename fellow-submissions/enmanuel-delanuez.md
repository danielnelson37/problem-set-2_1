# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
    - A unary operator performs an action to a single operand. An example of a unary operator is the `! : logical NOT operator`. It can be used like so: `!true === false`

2. What is a _binary operator_? Give an example of one.
    - A binary operator functions with two operands. Binary operators include *arithmatic operators* and *equality operators*, because while their function may differ they take two operads like so: `15 % 4`.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
    - The ternary operator takes three operands. Ternary operators is used to simplify *if...else* statements like so:
    ```
      let isCorrect = true;
      isCorrect ?
      console.log('Correct!'):
      console.log('Incorrect!');
    ```
This code snippet declares a variable with the boolean value `true`. The ternary operator `?` takes the first operand `isCorrect` preceeding it and determines whether it is or *truthy* or *falsy*. If truthy, the operand to following it will be executed. Else, the operand following `:` will be executed.

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
    - *Strict* equality operators only evaluate their operands if they are of the same data type. *Abstract*, or *non-strict* equality operators will coerce their operands to match data types as best it can before comparing.

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
    - The seven JS data types are:
      - Number: numbers, integers or decimals.
      - String: characters sorrounded by quotation marks.
      - Boolean: binary, true or false states.
      - Null: purposeful absense of data, analogous to an empty box.
      - Undefined: absense of data, analogous to no box where there should be.
      - Symbol: unique identifier.
      - Object: collection of related data.
  ---
  The first 6 data types in this list are considered *primitive* for they are built in.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
  This code returns 'string' because the unary operator `typeof` will evaluate the data type of the operand which is a set of characters inside quotation marks.

7. What does the code below return?
  ```javascript
  typeof true;
  ```
  This code returns 'boolean' because the unary operator `typeof` will evaluate the data type of the operand which is a boolean state of true or false.

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
  This code returns 'number' because the unary operator `typeof` will evaluate the data type of the operand which is numbers that are themselves operands of a binary arithmatic exponential operator.

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
This code returns 'null' because while `null` is not an object, this seems to be a bug in JS.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
    - *Truthy* and *falsy* are the inherit boolean values of different data types that come to light when other data types are converted or coerced to boolean. The six  *falsy* values that evaluate to `false` are:
      - `false`: the boolean state itself
      - `0`: zero
      - `''` or `""`: an empty string
      - `null`
      - `undefined`
      - `NaN`: not a number
      ---
      Everything else evaluates to true.

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null`
    - Arithmatic operator `*` coereces null to the number 0 and returns `0`.
  * `"5" - 1`
    - Arithmatic operator `-` coerces `"5"` to the number 5 and returns `4`.
  * `"5" + 1`
    - Arithmatic operator `+` coerces `"5"` to the number 5 and returns `6`.
  * `true + false`
    - Arithmatic operator `+` coerces `true` and `false` to the numbers 1 and 0 respectively and returns `1`.
  * `"i am" + undefined`
    - Operator `+` will concate in this case and coerce `undefined` to a string and return `"i amundefined"`.
  * `5 + undefined`
    - Arithmatic operator `+` will attempt mathematical operation for one operand is a number but fails when it encounters `undefined` and returns `NaN`.

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
  This line will return `false` because the *AND* operator checked if the first operand can be converted to *true*, it can't, so it returns the first operand `false`.

   ```javascript
   (false || undefined);
   ```
  This line will return `undefined` because the *OR* operator checked if the first operand can be converted to *true*, it can't, so it returns the second operand `undefined`.

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
  This line will return undefined following the logic above and evaluating inside out.

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
  `false`

   ```javascript
   ((false && undefined) && (false || undefined));
   ```
  `false`

   ```javascript
   ((false || undefined) && (false && undefined));
   ```
  `undefined`
  
   ```javascript
   ('a' || (false && undefined) || '');
   ```
  `a`

   ```javascript
   ((false && undefined) || 'a' || '');
   ```
   `a`
   ```javascript
   ('a' && (false || undefined) && '');
   ```
  `undefined`
  
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
  `undefined`
