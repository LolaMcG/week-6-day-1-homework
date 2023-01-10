1. The murderer is Miss Scarlett.
When the declareMurderer() function is called it is able to access the scenario variable because this variable is declared outside of the function, and at a global level, and is therefore accessible.

2. The murderer is Prof. Plum.
The changeMurderer() function is called but it can't actually do its job as it's declared at the start as a const variable so its value can't be reassigned. When the declareMurderer() function is called, therefore, it will access the original variable value it was given and return that i.e. Prof. Plum.

3. First verdict: the murderer is Mrs Peacock, second verdict: the murderer is Prof. Plum.
The declareMurderer() function is called and the results assigned to the firstVerdict variable. Within the declareMurderer() function the value of the murderer variable is reassigned, which is allowed as it uses the 'let' keyword. This new value only exists on  a local level, though, within the function. The secondVerdict variable is looking for the value of the murderer variable, and the only value that exists on a global level is Prof. Plum.

4. SuspectThree is Mrs Peacock.
SuspectThree IS reassigned the value of Colonel Mustard, but on a local level within a function. When the final console.log function is called, it will search for the suspectThree variable and replace ${suspectThree} with it's value. It cannot access the local level Colonel Mustard so will grab global Mrs Peacock instead.

5. The weapon is the Revolver.
The changeWeapon() function is called, passing in the Revolver argument. This function will reassign the value of scenario.weapon to whatever argument is passed into it. It's able to access the value of the weapon key as the scenario variable is declared on a block level. The declareWeapon() function is then called and will look at the value of the weapon key in the scenario variable, which was just changed to Revolver.

6. The murderer is Mrs White.
The changerMurderer() function is called. This function first reassigns the value of the murderer variable to Mr Green, then defines a new function called plotTwist which reassigns the murderer variable to Mrs White, and THEN calls that function, so the murderer is now Mrs White. The value is able to be changed as the murderer variable uses the let keyword. The changeMurderer() function is called at the bottom, then the declareMurderer() function, which looks for the murder variable and returns a string with its value in it.

7. The murderer is Mr Green. The murder variable is set at Prof. Plum, then the changeMurderer() function is called which reassigns this value to Mr. Green. Two more functions are defined and called within the changeMurderer() function, but the value of their murderer variables only exist within this function and not outside it. So when the declareMurderer() function is called it will look for the value of the murderer variable, which is now Mr Green as it just vhanged by the changeMurderer() function.

8. I got so lost with this one.

9. The murderer is Prof. Plum.
The global varibale Prof. Plum is declared. Then, within the if block, a local variable, also called murderer, is declared, but it exists only on a local level within the if statement therefore doesn't affect the value of the global murderer variable, Prof. Plum.