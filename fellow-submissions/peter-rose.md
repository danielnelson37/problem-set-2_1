# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.

    A Unary Operator is a single operator that performs than an operation. An example of this is the logical not (!) or incremental 
    operators such as ++ or --.
    
2. What is a _binary operator_? Give an example of one.

    A Binary Operator is an operator that requires 2 operands to perform it's tasks.
    
    Ex: console.log(5 + 5)

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
 
    A Ternary Operator requires 3 operands in order to perform its operation. It is also
    used as shorthand for an if statement.

    Ex: 
    let food = `true`
    let didEat = food ? 'Yeah im full!' : 'I'm starving!!!'; 
    // 'Yeah I'm back'

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
    
    When using a strict operator those values will only be equal if the type AND value is equal rather
    than it just being of the value.

    This is the difference between ("5" == 5) and (5 === "5")
                                    //true         //false

5. What are the seven JavaScript data types? Which of these are considered _primitive_?

    JavaScript is conprised of 2 main types of data, which are primitives, and objects. 
    A primitive is simply a data type that is not an object, and has no methods. Usually these cannot be changed after they are initiazed.
    The primitive data types are string, number, boolean, symbol , and undefined.

6. What does the code below return?
  ```javascript
  typeof 'I love marcy lab';
  ```
    --> //string

7. What does the code below return?
  ```javascript
  typeof true;
  ```
    --> // Boolean

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
    --> // Number
    The output would be "Number" rather than the value of the expression which would be 1,000,000,000.

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
    --> object

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

    A truthy is a value that will be evaluate as true when coerced into a boolean.
    This is useful for developers if you want to check if a variable exists within your code or reference it in some context.
    The falsy values are undefined, "", false, NaN, null, and 0,
    
    if (1997) --> true.
    if ("0") --> true, even though would normally be false if it was a number rather than string.
    if ("false") --> true.

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null` // null to number. 8 * 0 = 0
  * `"5" - 1` // String to number --> 4
  * `"5" + 1` // Number to string --> 51
  * `true + false` //booleans to numbers b/c of the + operator. true + false = 1. Same as 1 + 0 = 1. 
  * `"i am" + undefined` //undefined to string. output = "i amundefined"
  * `5 + undefined` // NaN, Js doesnt recoginize undefined as a number.
  * 

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
   --> false



   ```javascript
   (false || undefined);
   ```
    --> false



   ```javascript
   ((false && undefined) || (false || undefined));
   ```
    --> false
    
    
    
   ```javascript
   ((false || undefined) || (false && undefined));
   ```
    --> false
    
    
    
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
    --> false
    
    
    
   ```javascript
   ((false || undefined) && (false && undefined));
   ```
    --> undefined
    
    
    
   ```javascript
   ('a' || (false && undefined) || '');
   ```
    --> true 'a'



   ```javascript
   ((false && undefined) || 'a' || '');
   ```
    --> true 'a'
    
    
    
   ```javascript
   ('a' && (false || undefined) && '');
   ```
   --> undefined
   
   
   
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
    --> undefined