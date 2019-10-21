# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
Answer: A _unary operator_ is an operator that takes one operand. For example the logical operator (not !).

2. What is a _binary operator_? Give an example of one.
Answer: A _binary operator_ is an operator that takes two operands. For example the logical operator (and &&).

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
Answer: We use the _ternary operator_ with 3 operands and want to ask a question(?) and return a value based on a condition.
`console.log(true ? 1 : 2);`
` output:1`


4. What is the difference between using the _strict_ and _non-strict_ equality operators?
Answer: The difference between using _strict_ and _non-strict_ equality operators is we use _strict_ equality operator when comparing  on operands that must be the same type otherwise it will return false. We use _non-strict_ when comparing operands even if they are not of the same type and coerce to be the same type.

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
  * `8 * null`  = 0 because null is coerced to 0 and 8 * 0 is 0.
  * `"5" - 1`  = 4 because the substract operator coerces both operands to numbers before performing the operation.
  * `"5" + 1` = "51". Because "5" is a string, the addition operator will coerce both operands to string and concatenate them.
  * `true + false` = 1 because true is coerced to 1 and false is coerced 0 so 1 + 0 = 1.
  * `"i am" + undefined` = "i amundefined " because "i am" is a string and the addition operator coerced them.
  * `5 + undefined` = NaN because The addition operand will coerce undefined to a number. Undefined coerces to Nan. Anything plus undefined will return NaN.

12. What will each line of the following code return?
  
   ```javascript
   (false && undefined);
   ```
Answer: false

   ```javascript
   (false || undefined);
   ```
Answer: undefined

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
Answer: undefined    
   

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
ANswer: false

   ```javascript
   ((false && undefined) && (false || undefined));
   ```
Answer: false 

   ```javascript
   ((false || undefined) && (false && undefined));
   ```
Answer: undefined    
   
   ```javascript
   ('a' || (false && undefined) || '');
   ```
Answer: a   

   ```javascript
   ((false && undefined) || 'a' || '');
   ```
Answer: a       
   
   ```javascript
   ('a' && (false || undefined) && '');
   ```
Answer: undefined
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
Answer: undefined