# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
    A unary operator is a named operator that takes only one operand, one example would be typeof
    which detects what type a piece of data is.

2. What is a _binary operator_? Give an example of one.
    A binary operator  is a named operator an operator that takes two operands, 
    one example would be && which returns only if both items are true.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below?
    named operator that is a conditional, 
    console.log(true ? 1 : 2);
    // → 1
    based on first value it picks which value to output

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
    The difference between the strict and non-strict equality operators is based on how direct one needs to compare value. 
    One compares just the values ( == ) and through coercion changes the type of data 
    while the other ( === ) compares both the value and its type which can be crucial for certain applications.

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
    The seven JavaScript data types are:
        number
        string
        boolean
        object
        null
        undefined
        typeof

        Of these undefined,null,boolean,string,and number are considered primitive.

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
    It returns string since that is a string.

7. What does the code below return?
  ```javascript
  typeof true;
  ```
   It returns boolean since the value given was true.

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
    It returns number since the value that is returned after the operation is a number.

9. What does the following code return? Why?
  ```javascript
  typeof null;
  ```
   It returns object. Null is an object that denotes no value. Essentially a value that has no value.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

     In JavaScript truthy and falsy are basically comparisons of values when coercioned to their boolean equivalent of either true or false.
     All values are considered truthy unless they are defined otherwise. 
     The six values considered falsy are:
         false
         null
         undefined
         0
         NaN
         ''

11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null` (0)   Read 8 * 0 in javascript
  * `"5" - 1` (4)    Read 5 - 1 in javascript
  * `"5" + 1` (51)   Read "5" + "1" in javascript
  * `true + false` (1)   Read 1 + 0 in javascript
  * `"i am" + undefined` ("i amundefined")   Read "i am" + "undefined" in javascript
  * `5 + undefined` (NaN)    Don't add null or undefined to numbers they don't mean anything.
  
    JavaScripts implicit coercion riles dictate that JavaScript will try to convert data types to a value that make sense.
    Adding to a string will just add to a string.  If a number can be given based on a type having an equivalent number value,
    that will be used instead.

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
    It returns false,since both false and undefined are not true.

   ```javascript
   (false || undefined);
   ```
    It returns undefined since || stands for or and as a value false is not 'true' as a value.

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
   It returns undefined since the first  statement is not true and the second is the same as the one above.

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
    It returns false since both statements are both false.
    
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
    It returns false since the first statement is not true so it cannot compare to the other statement.
    
   ```javascript
   ((false || undefined) && (false && undefined));
   ```
    It returns undefined because it compares a statement that returns undefined and one that is false.
    
   ```javascript
   ('a' || (false && undefined) || '');
   ```
    It returns 'a' since the second statement is not true and the third is an empty string aka no value.
    
   ```javascript
   ((false && undefined) || 'a' || '');
   ```
   It returns 'a' for the same reasons as the question above, an empty string holding no value 
   and the other statement is false.

   ```javascript
   ('a' && (false || undefined) && '');
   ```
    It returns undefined because this is comparing muliple types while also having a statement that has a value of undefined.
    
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
    It returns  undefined for the same reason as above. A string with no value , 
    a string with value,both compared with a statement that holds the value of undefined.