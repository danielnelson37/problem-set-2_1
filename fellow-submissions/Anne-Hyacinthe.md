# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
    * An _unary operator_ is an operator which takes only one operand. An example of this is the _unary plus_ which uses conversion to change a string into a number. The format for an _unary operator_ is an adition sign in front of an operand. 

2. What is a _binary operator_? Give an example of one.
    * A _binary operator_ is an operator which takes two operands. An example of this is the _greater than operator_ which  purpose is to compare two operands. 

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
    * A _ternary operator_ is used when a condition is short enough to logically fit into one line

4. What is the difference between using the _strict_ and _non-strict_ equality operators?

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
    * The seven type of JavaScript data types are numbers, string, boolean, null undefined, symbol and objects. The first six data types are all primitive.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
   *string
7. What does the code below return?
  ```javascript
  typeof true;
  ```
    *Boolean
8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
    *numbers
9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
    *null
10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
    *_Truthy_ is when an operand is true and a _falsy_ is when an operand is false. 

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null`
        JavaScript will use coercion to make it null therefore making the answer 0.
  * `"5" - 1`
        JavaScript will use coercion to make `"5"`, a string to 5, a number and the solution will be 4.
  * `"5" + 1`
        JavaScript will use coercion to make 1, a number to `"1"`, a string and the solution will be "51".
  * `true + false`
        JavaScript will use coercion to make it 1 because true equates to 1 and false equates to 0 making the equation 1 + 0 and the solution 1.
  * `"i am" + undefined`
        JavaScript will use coercion to make it "i amundefined" because "i am" is a string it automatically concatenate with `undefined`.
  * `5 + undefined`
        JavaScript will use coercion to make the solution Nan because it will make undefined Nan and Nan plus 5 is still Nan.

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
     false
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
    false
   ```javascript
   ((false || undefined) && (false && undefined));
   ```
    undefined
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
    false
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
    undefined