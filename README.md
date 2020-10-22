# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.
 
   An unary operator is a single operand and this operator comes before or after the operator . An example of one is ++.

2. What is a _binary operator_? Give an example of one. 

    Binary operator has different symbols from the unary and has 2 operand one before and one after. An example of one is +.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below. 

    We use ternary operator when we want to run a code block based on a condition. (condition) ? result1: result2. The code block would run the first condition if the 1 result1 comes out flasy it run will run the 2nd code. 

4. What is the difference between using the _strict_ and _non-strict_ equality operators? 

    The difference between strict and non-strict is that strict compare data type as well as value and non-strict ignore data type but they must have matching numbers. 


5. What are the seven JavaScript data types? Which of these are considered _primitive_? 
    The seven javaScript data types are number,string,boolean,undefined,null,object and symbol.


6. What does the code below return?
    
    The code below return a string.
  ```javascript
  typeof 'i love marcy lab';
  ```

7. What does the code below return?

    The code below return boolean.
  ```javascript
  typeof true;
  ```

8. What does the code below return?

    The code below return number.

  ```javascript
  typeof (10**9);
  ```

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

    Truthy means that the value of the code is true and falsy means that the value of the code is false. Six values of falsy is null,0,NaN,undefined, empty string and false.


11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why: 

    
    
  * `8 * null`
  * JavaScript can't reslove the operator so it performs type coercion because null is not a number there by it converts it to 0, than it muitply 8 by 0 and gets 0. 

  * `"5" - 1` 
   * javaScript can't handle string values so it's gonna convert the string into a number using type coercion. 
  
  * `"5" + 1`
    * the only operator javaScript can handle on strings is the addition operator and perform type coercion on the 1 than it concates on to a string.
  
  * `true + false` 
    * becuase javaScript can not handle the addition of two booleans it performs type coercion on them which true results to 1 and false results into 0 then you could combine the two. 
  
  * `"i am" + undefined` 
     the only operator javaScript can handle on strings is the addition operator and perform type coercion on the undefined than it concates on to a string.
    
  * `5 + undefined`
   * javaScript tries to perform type coercion on undefined but it results in NaN and when javaScript performs addition on a number and NaN it becomes NaN.
 


12. What will each line of the following code return?
   ```javascript
   (false && undefined); 
   
    false
   ```

   ```javascript
   (false || undefined); 
   
    undefined
   ```

   ```javascript
   ((false && undefined) || (false || undefined)); 
    undefined
   ```

   ```javascript
   ((false || undefined) || (false && undefined)); 
    false
   ```

   ```javascript
   ((false && undefined) && (false || undefined)); 
    false
   ```

   ```javascript
   ((false || undefined) && (false && undefined)); 
    undefined 
   ```

   ```javascript
   ('a' || (false && undefined) || '');
   ``` 
    "a"

   ```javascript
   ((false && undefined) || 'a' || '');
    "a"

   ```javascript
   ('a' && (false || undefined) && ''); 
   "undefined"
   ```

   ```javascript
   ((false || undefined) && 'a' && ''); 
   "undefined"
   ```
