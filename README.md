# Problem Set 2.2 - Variables and Control Flow
## Short Response Questions

1. **What does the code below log? Why?**
   ```javascript
   {
      let singer = 'Omar Apollo';
   }

   console.log(`My favorite singer is ${singer}`); 
   ```
       The code below would log error because Omar Apollo was declared inside a block and cannot be accessed from outside the block

2. **What happens when we run the following code? Why?**
   ```javascript
   const favorite = 'Juan Pablo';
   console.log(`Our favorite Marcy Lab family member is ${favorite}!`); 
      

   favorite = 'Maya';
   console.log(`Actually, ${favorite} is my favorite.`); 
   ```
      When we run the following code Juan Pablo would be the marcy lab favorite family member because it is declared to be Juan Pablo. 
     When you resign a value to constant it would come out as an error because we assign primitive value to a constant, we cannot change the primitive value.

3. **What does the following code log? Why?**
   ```javascript
   let score = 90;
   let newScore = score;
   score = 100;
   console.log(score, newScore); 
   ``` 
   The following code would log 100 90. On line 1, the variable score is declared and initialized to a value of 90. One line 2, the variable newScore is declared and also initialized to the value of score, which is 90. On line 3, score is reassigned to a value of 100, while newScore is not changed.

4. **Why doesn't the following code log an uppercase string? Change the code so that it does.**
   ```javascript
   let greet = 'hello';
   greet.toUpperCase();
   let scream = greet;
   console.log(scream);
   ```
   On line 1, the variable greet is declared and initialized to a value of "hello". On line 2, we invoke a function toUpperCase to create a new uppercase string, but that data is never stored. The original string cannot be mutated (cannot change). On line 3, the variable scream is declared and initialized to the value stored in greet which is still the string "hello". When we console.log scream, we see "hello".

To make the code work, we should change line 3 to: let scream = greet.toUpperCase().
   

5. **What does the following log? Explain why, ensuring to explain how `someName` and `busy` were declared?**
   ```javascript
   let name;
   let nickname = 'ghost';
   let someName = name || nickname;
   let children = null;
   let homework = 'lots';
   let busy = children && homework;

   someName ? console.log(`${someName} evaluates to true`) : console.log(`${someName} evaluates to false.`); 
   busy ? console.log(`${busy} evaluates to true`) : console.log(`${busy} evaluates to false.`);
   ```
      someName is assigned nickname because it was the first truthy value in the or operator. So someName becomes ghost.
      busy is assigned children because it was the first falsey value in the operator. So busy becomes null.

6. **The following code causes an infinite loop. Why?**
   ```javascript
   let counter = 0;

   while (counter <= 5) {
     counter = 1;
     console.log(`count: ${counter}`);
     counter += 1;
   } 
   ```
      The code causes a infinite loop because counter is set to 1 and there is no way counter would be greater than 5 because it keeps on getting push to 1.
