# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
    A unary operator works with only one argument to change it's result
        Ex:
            "!true"
            will output false

2. What is a _binary operator_? Give an example of one.
    A binary operator works with two arguments to change it's result
        Ex:
            "4+2" 
            will output 6 because it is taking in 4 and 2 as arguments and adding them to provide a result

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
    The ternary operator is like a simplified if else statement. It takes the condition first followed by a "?". 
    After that it will have an expression that will run if the condition is true, it is then followed by a ":" with
    an expression that will run if the condition turns out to be false.
                Ex:
                4>5 ? "Yes, 4 is greater than 5": "No, four is not greater than 5"
                This will output "No, four is not greater than 5", because the condition "4>5" is false

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
    When using a _non-strict_ equality operator the two things that are being "compared" should have the same content but
    can have different data types, it also uses a double equal sign "=="
        Ex:
            '5' == 5 
            Will output true, even though the first argument is a string and the second is a number.It will automatically do
            coercion and turn the string/number 5 to match the other 5
    While the _strict_ equality operator requires both arguments to have the same data type and same content, it uses three 
    equal signs "==="
        Ex: 
            '5'===5
            Will output false because the string 5 doesn't equal the number 5.This does not do coercion if you want to compare 
            both you will have to do conversion so that they have the same data type

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
    The seven JavaScript data types are:
        1)Number _primitive_
        2)String _primitive_
        3)Boolean _primitive_
        4)Null _primitive_
        5)Undefined _primitive_
        6)Symbol _primitive_
        7)Object
    
6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
    It will return "string"

7. What does the code below return?
  ```javascript
  typeof true;
  ```
     It will return "boolean"

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
     It will return "number"

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
     It will return "object", because they have the same type tag

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
    _truthy_ is anything that when turned to a boolean value is true, while _falsy_ values is anything that when turned to a boolean
    value it is false
    These are the falsy value:
        1)false 
        2)undefined
        3)null
        4)empty strings
        5)0
        6)NaN

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null` : 0, null was coerced into 0 because it has an empty value
  * `"5" - 1` : 4, the string "5" was turned into a number because it is trying to subtract 1 from the string 5
  * `"5" + 1` : 6, the string "5" was turned inot a number because it is trying to add 1 to the string 5
  * `true + false` : 1, both true and flase boolean values are turned into numbers so that the addition operator can take place
  * `"i am" + undefined`: "i amundefined", because the addition sign is also used to append strings together and the first value is a string,
                          and the second is a falsy in order for it to be added it will have to turn into a string
  * `5 + undefined` : NaN, because 5 is a number and undefined isn't a number and can't be turned to a number even if it is coerced,
                      so when they are trying to be added it will give NaN

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ``` 
   This will return:
            False
   ```javascript
   (false || undefined);
   ```
    This will return:
            undefined
   ```javascript
   ((false && undefined) || (false || undefined));
   ```
    This will return:
            undefined

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
   This will return:
            false
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
   This will return:
            false

   ```javascript
   ((false || undefined) && (false && undefined));
   ```
   This will return:
            undefined

   ```javascript
   ('a' || (false && undefined) || '');
   ```
   This will output:
            'a'

   ```javascript
   ((false && undefined) || 'a' || '');
   ```
    This will output:
            'a'
   ```javascript
   ('a' && (false || undefined) && '');
   ```
    This will output:
            unefined
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
   This will output:
            undefined
