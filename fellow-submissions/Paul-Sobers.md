# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
Answer: An _unary operator_ is an operator that takes one value. For example the logical operator (not !).

2. What is a _binary operator_? Give an example of one.
Answer: A _binary operator_ is an operator that takes two values. For example the logical operator (and &&).

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
Answer: We use the _ternary operator_ when we have 3 values and want to ask to return a value base on the boolean value on the left.
`console.log(true ? 1 : 2);`
`// → 1`


4. What is the difference between using the _strict_ and _non-strict_ equality operators?
Answer: The difference between using _strict_ and _non-strict_ equality operators is we use _strict_ equality operator when performing comparison on operands  of the same type. We use _non-strict_ when comparing operands even if they are not of the same type.

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
Answer: The seven JavaScript data types are `Strings` ,`Number`,`Boolean`,`Null`,`Undefined`,`Object`,and `Symbol`. `Strings`,`Number`,`Boolean`,`Null`,`Undefined` are considered _primitive_.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
Answer: This code will return: `'String'` because of the `typeof` operator that checks the value to its right and return a string of its data type.

7. What does the code below return?
  ```javascript
  typeof true;
  ```
Answer: This code will return: `'Boolean'` because true is a value of the data type Boolean.

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
Answer: This code will return: `'Number'`.  

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
Answer: This code will return : `'Object'` because since the first implementation of JS , JavaScript values were labeled as type tag and a value. The type tag for objects was 0. null had 0 as a type tag that is why typeof return object instead of 0 because it return a string of its data type.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
Answer: To be _truthy_  is a value that is considered to be true and _falsy_ is a value that is considered to false. Everything is considered true unless you set that value to false. The six values of _falsy_ are `False`,`0`,`""`,`null`,`undefined`,and `Nan`.

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
Answer: 


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
