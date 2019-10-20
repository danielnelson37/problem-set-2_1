# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
	A unary operator is a single argument that performs an operation. An example of this would be the 'typeof' operator which takes in an operand and returns the value. 

2. What is a _binary operator_? Give an example of one.
	A binary operator takes in two operands to perform an operation. 
An example of this is arithmetic operators such as, -, /, %, *, which take in two operands to return a value. 

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
	The ternary operator is the only operator that takes in three operands. It is a shortcut to the if-else statement.  

        person.driver =(person.age>= 16? 'yes' : 'no';)
        
        Here you are asking if the driver's age is greater than or equal to 16. if it is you return the first value which is 'yes' if it is not true, you have to take in the second value. 

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
	A strict equality operator such as ‘===’  is only true if the operands are the same data type and the content of the operands match. 
    A non-strict equality operator such as, ‘==’ is a more abstract comparison that converts the operands to the same type to and checks that the contents match.


5. What are the seven JavaScript data types? Which of these are considered _primitive_?
    There are six primitive data types those are:
        1.String - a collection of characters 
        2.Number - an integer
        3.Boolean - true or false 
        4.Null - the absence of data
        5.Undefined - data is not there yet
        6.Symbol - unique primitive value  
    The seventh data type is an object. Objects are data types you can create.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
   This will return 'string' because it is in '' quotes. 

7. What does the code below return?
  ```javascript
  typeof true;
  ```
    This will return 'boolean' because 'true' is a boolean property

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
    This will return 'number' because 10 and 9 are integers being used with an arithmetic operator

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
  This will return 'object' because null is the absence of data and 'object' stands for the beginning of JavaScript 

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
    When something is truthy it means it is not one of the six falsy values.
    A falsy value is: 
        1.The boolean ‘false’
        2.The number 0
        3.Any empty string 
        4.Null
        5.Undefined
        6.NaN


11. Evaluate the following expressions using JavaScripts’ implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null`
This will return 0 because it coerced null to the number 0 and any number multiplied by 0 is zero. 
	
  * `"5" - 1`
This will return 4 because it coerced the string ‘5’ to the number 5 and 5-1 is 4. 

  * `"5" + 1`
This will return ‘51’  because it coerced the number  1 to a string and added that value to the string ‘5’.

  * `true + false`
This will return the number 1 because the boolean ‘true’ is coerced to the number 1 and ‘false’ is coerced to the number 0 resulting in 1 + 0 which is 1. 

  * `"i am" + undefined`
This will return ` ‘i amundefined’ ` since undefined is coerced to a string and is being added to the string ‘i am’.

  * `5 + undefined`
This will return NaN, because undefined can not be coerced to a number, therefore, 5+undefines is not a number. 

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
    'false', this because the AND logical operator will consider both the first and last operand to be truthy to return ‘true’. Since the first operand is false,  the second is not considered and this will automatically return false.

   ```javascript
   (false || undefined);
   ```
   'undefined', this is because this is a logical OR operation. It will consider both operands in it’s a statement and if one of them is truthy or more than one, it will return the first truthy. If all operands in a logical OR operation are falsy it will return the last operand. Since all both operands were falsy it returned ‘undefined’ which was the last operand.

 ```javascript
   ((false && undefined) || (false || undefined));
   ```
    'undefined', because the first statement is false and the second is undefined, but they are in a logical OR operator which will return the last operand if they are both falsy. 
  
 ```javascript
   ((false || undefined) || (false && undefined));
   ```
    'false', because the first statement is undefined and the second is false, but they are in a logical OR operator which will return the last operand if they are both falsy. 
  
 ```javascript
   ((false && undefined) && (false || undefined));
   ```
    False, the first statement is false and the second statement is in a logical OR operation so it is undefined, but these are both in a logical AND operation which will return false since the first operand was falsy. 
  
 ```javascript
   ((false || undefined) && (false && undefined));
   ```
    Undefined, this is because the first statement is in a logical OR operation and will return the last operand which is undefined. The second statement is in a logical AND operation so it is false, since the first operation is false. However, these are both in a logical AND operation which will return undefined since the first operand was ‘undefined’, a falsy value.
    
```javascript
   ('a' || (false && undefined) || '');
  ```
   'a' is returned, this is because this statement is a logical OR operation, and if any of these operands are truthy it will return the first truthy even if the other operands are falsy.    
```javascript
   ((false && undefined) || 'a' || '');
  ```
  'a' is returned, this is because this statement is a logical OR operation, and if any of these operands are truthy it will return the first truthy, which in this statement is the second operand even if the other operands are falsy. 
   
```javascript
   ('a' && (false || undefined) && '');
  ```
   Undefined will be returned. This statement is a logical AND operation, which will consider all operands to be truthy to return ‘true’. Since the first operand is ‘a’ it is true, the second operand is in a logical OR operation which returns undefined because it is the last operand of two falsy operands. The third operand is not considered since the second operand was a falsy value and this will automatically return the second operand which was undefined.

  
 ```javascript
   ((false || undefined) && 'a' && '');
   ```
  Undefined will be returned. This is a logical AND operation, which will consider all operands to be true in order to return ‘true’.  Since the first operand is a logical OR operation, it will consider both operands in it’s a statement and if one of them is truthy or more than one, it will return the first truthy. If all operands in a logical OR operation are falsy it will return the last operand. Since all both operands were falsy it returned ‘undefined’ which was the last operand. Undefined is a falsy value and was the first falsy value in the logical AND operation which was imminently returned. 
