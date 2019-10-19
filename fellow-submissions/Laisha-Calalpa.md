# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
    A _unary operator_ is an operator that takes a single operand and performs an operation.  
    An example would be the typeof operator which produces the type of a single operand. 

2. What is a _binary operator_? Give an example of one.
    A _binary operator_  is an operator that takes in two operands that produce a single operand. 
    Logical operators are an example of such as they compare two operand and then execute to a single argument 

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
        The _ternary operator_ is a shorthand for an if else statement. 
    ```
    (weather === “sunny”)
    weather ? console.log(“go outside!”) : console.log(“stay inside!”);
    ```

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
    The `strict` equality operator does not allow for non-equal values to undergo coercion.
    While _non-strict_ equality operators allow for coercion to occur with different data types 
    in order to execute the command. 

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
    The seven JavaScript data types are `number`, `string`, `boolean`, `null`, `undefined`,`symbol`.
    All data types excluding `symbol` are considered primitive data types.

6. What does the code below return?
    ```
    javascript
    typeof 'i love marcy lab';
    ```
    The code returns `string`.

7. What does the code below return?
    ```
    javascript
    typeof true;
    ```
    The code returns `boolean`. 

8. What does the code below return?
    ```
    javascript
    typeof (10**9);
    ```
    The code returns `number`.

9. What does the following code return? Why?
    ```
    javascript
    typeof null;
    ```
    The code returns `object` because null has a 0 type tag that corresponds to an object. 

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
    Being _truthy_ means that value is a value that is true and a _falsey_ is a value that evaluates to false. 
    The six _falsy_ are `false`, `null`, `undefined`, `""`, `0`, `NaN`, 
    
11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null`
    The expression evaluates to `number` 0 as the value of null is 0 and is multiplied by 8 through coercion the code executes to 0. 
  * `"5" - 1` 
    The expression evaluates to `number` 4 because the math operand of subtraction causes the string value to be coerced into a number data type and then executes 5-1.  
  * `"5" + 1`
    The expression evaluates to `string` 51 due to string being the first value that is followed by '+' operand which is considered for concatenation instead of addition. 
  * `true + false`
    The expression evaluates to `number` 1 because true holds the value of 1 and false holds the value of 0, this would have the expression be 1 + 0 executing to 1. 
  * `"i am" + undefined`
    The expression evaluates to `string` i amundefined because undefined is coerced imto a string and the '+' opperand is considered concatenation. 
  * `5 + undefined`
    The expression evaluates to `NaN` since undefined has the value of not a number, no operation can be performed and NaN cannot be coerced . 
12. What will each line of the following code return?
    ```
    javascript
    (false && undefined);
    ```
    `false`

    ```
    javascript
    (false || undefined);
    ```
    `undefined`
    
   ```
   javascript
   ((false && undefined) || (false || undefined));
   ```
   `undefined`
   
   ```
   javascript
   ((false || undefined) || (false && undefined));
   ```
   `false`

   ```
   javascript
   ((false && undefined) && (false || undefined));
   ```
    `false`
    
   ```
   javascript
   ((false || undefined) && (false && undefined));
   ```
   `undefined`
   
   ```
   javascript
   ('a' || (false && undefined) || '');
   ```
   `a`

   ```
   javascript
   ((false && undefined) || 'a' || '');
   ```
   `a`

   ```
   javascript
   ('a' && (false || undefined) && '');
   ```
   `undefined`
   
   ```
   javascript
   ((false || undefined) && 'a' && '');
   ```
   `undefined`
