# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.

2. What is a _binary operator_? Give an example of one.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below.

4. What is the difference between using the _strict_ and _non-strict_ equality operators?

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

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

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
