# Problem Set 2.1
## Types, Values, and Operators

1. What is _unary operator_? Give an example of one.  
 ``` 
 A unary operator take in an argument and runs the operation.
 example is logical Not(!) it use to represent not in javascript.
 ```
2. What is a _binary operator_? Give an example of one.  
 ```
 A binary requires two command on both side and execute the code. 
 example of binary operator is && which is and,the and operator will check
 if the code on both sides are true.
 ```
3. When do we use the _ternary operator_? Use a code snippet to illustrate below. 
```
We can use ternary operator when we want to simplify our code instead of using if else statement.  
  If else:  
  if (2 > 3) {                         
      console.log(true)                        
  } else {\
      console.log(false) \
  } \
      Tenary operator:  2 > 3 ? true : false
```
4. What is the difference between using the _strict_ and _non-strict_ equality operators?  
```     
Strict equality operator checks the value and the class 
while non-strict just checks if the value is the same and outputs true
```
5. What are the seven JavaScript data types? Which of these are considered _primitive_?  
```     
     Primitive:  
     Undefined  
     Boolean  
     Number  
     String  
     BigInt  
     They are called primitive because they can't be directly mutated but they can be replaced.\
       Symbol 
```
6. What does the code below return?  
  ```javascript
  typeof 'i love marcy lab';
  ```
```
  String
```
7. What does the code below return?  
  ```javascript
  typeof true;
  ```
```
  Boolean 
```
8. What does the code below return?  
  ```javascript
  typeof (10**9);
  ```
```
   Number 
```
9. What does the following code return? **Why**?  
  ```javascript
  typeof null;
  ```
```
   Object  
```
10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?  
```
Truthy means that it is pretty close to being true. while falsy means that is pretty close to being 
false.  
     Falsy:  
            False	The word false  
            0	The number zero
            -0	The number negative zero
            0n	BigInt, when used as a boolean, follows the same rule as a Number. 0n is falsy.
            ""	Empty string value
            null	null - the absence of any value
            undefined	undefined - the primitive value
            NaN	NaN - not a number
```
6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
  String\
7. What does the code below return?
  ```javascript
  typeof true;
  ```
  Boolean\
8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
   Number\
9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```
   Object\
10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?  
      ```
      Truthy means that it is pretty close to being true. 
      while falsy means that is pretty close to being false.
      Falsy:
          False	The word false
          0	The number zero
          -0	The number negative zero
          0n	BigInt, when used as a boolean, follows the same rule as a Number. 0n is falsy.
          ""	Empty string value
          null	null - the absence of any value
          undefined	undefined - the primitive value
          NaN	NaN - not a number
      ```
11. Evaluate the following expressions using JavaScripts implicit coercion rules. Then, in one sentence, explain what coercions were applied and why:
  * `8 * null`\
    ```
    0  data-type: number was applied because null was empty so it timesed 8 and
    returned 0 as the best guess.
    ```
  * `"5" - 1`\
    ```
    4  data-type: number was applied because the string 5 was coerced into number 
    5-1.
    ```
  * `"5" + 1`\
    ```
    "51"  data-type: String was applied because js thinks we are trying to join two strings.
    So the number 1 was coerced into a string
    ```
  * `true + false`\
    ```
    1 data-type: number was applied because it was easier 0= false 1= true the boolean
    were coerced into a number were true is 1 and false is 0.
    ```
  * `"i am" + undefined`\
    ```
    "i amundefined" data-type: string was applied because javascript thnks that the closest possible
    answer is adding two strings.Undefined was coerced into strings and added with i am.
    ```
  * `5 + undefined`\
    ```
    Nan  data-type: number was applied because it was easier and safer.Undefined was coerced into 
    a number which result in not a number because undefined is a word.
    ```
12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
    False
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
      False
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
      False
   ```javascript
   ((false || undefined) && (false && undefined));
   ```
      undefined
   ```javascript
   ('a' || (false && undefined) || '');
   ```
      "a"
   ```javascript
   ((false && undefined) || 'a' || '');
   ```
      "a"
   ```javascript
   ('a' && (false || undefined) && '');
   ```
     undefined
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
     undefined
