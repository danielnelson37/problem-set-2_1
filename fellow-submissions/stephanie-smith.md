# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
  A unary operator is a shortcut operator that acts just like the Number() object. It changes strings to numbers. Example: +("90");

2. What is a _binary operator_? Give an example of one.
  A binary operator requires two operands to fulfill a condition. Example: 3 + 4;

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
  We often use ternary  operators when setting values if a condition is true or if a condition is false. Example: return (isMember ? "$2.00" : "$10.00");


4. What is the difference between using the _strict_ and _non-strict_ equality operators?
  The abstract equality operator coerces, or guesses which type the data you're comparing before making the comparison.
  The strict equality operator does not coerce any of the values at all, so it will remain the type of data you inputted and make a comparison.

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
  Strings, integers, booleans, null, undefined, bigint, and symbol.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
  Expected output is string.

7. What does the code below return?
  ```javascript
  typeof true;
  ```
  Expected output is boolean.

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
  Expected output is an integer

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
  Expected output is undefined, because although the variable might have been declared, null is explicitly declaring the variable is undefined.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
  It's a cute term people use to describe values that equate as true or false. The six _falsy_ values are:
  - false
  - 0
  - Any empty string ("")
  - null
  - undefined
  - NaN (not a number)

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null` - Evaluates to 0. Null is equal to false, which is also equal to 0.
  * `"5" - 1` - Evaluates to 4. "5" is coerced into a number because there is a subraction of 1 rather than a plus.
  * `"5" + 1` - Evaluates to "51". The number is concatenated into the string "5", coerced into a character so it becomes "51" instead of 6.
  * `true + false` - Evaluates to 1. Both booleans coerce to numbers, true being 1 and false being 0. 1 + 0 is 1.
  * `"i am" + undefined` - Evaluates to "i amundefined". It seems like undefined is coerced into a string and concatenated to "i am".
  * `5 + undefined` - Evaluates to NaN. If there is an undefined type, the answer will not be a number, hence NaN.

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
  It will return false.

   ```javascript
   (false || undefined);
   ```
   It will return undefined.

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
   It will return undefined.

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
   It will return false.

   ```javascript
   ((false && undefined) && (false || undefined));
   ```
   It will return false.

   ```javascript
   ((false || undefined) && (false && undefined));
   ```
   It will return undefined.

   ```javascript
   ('a' || (false && undefined) || '');
   ```
   It will return "a".

   ```javascript
   ((false && undefined) || 'a' || '');
   ```
   It will return "a".

   ```javascript
   ('a' && (false || undefined) && '');
   ```
   It will return undefined.

   ```javascript
   ((false || undefined) && 'a' && '');
   ```
   It will return undefined.