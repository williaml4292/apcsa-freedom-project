# Tool Learning Log

## Tool: **Unreal Engine** (and C++ I guess)

## Project: **3D PVE RPG**


### 10/19/26:
* Found some tutorials for C++ online.
* [https://www.coursera.org/specializations/cplusplusunrealgamedevelopment](https://www.coursera.org/specializations/cplusplusunrealgamedevelopment)
* [https://www.codecademy.com/learn/learn-c-plus-plus](https://www.codecademy.com/learn/learn-c-plus-plus)

* Can probably learn C++ at school and tinker with Unreal at home.
---
### 10/23/26:
* The first link requires a subscription after 7 days.
* Codecademy has free lessons.

C++ is a general-purpose coding language that can be used anywhere.
It has the standard way of running--top to bottom.

* File naming: fileName.cpp
  * .cpp = C Plus Plus
* File Structure:
  * 1) Include libraries
    2) main function
    3) Beginning of main function
    4) code
    5) End of main function.
`std::cout << "Hello World!\n";`
* `std::cout` stands for **c**haracter **out**put stream (called see-out)
  * `<<` comes after it.
  * Things in the quotes are being output.
  * \n is new line.
  * ; = end of statement.
``` C++
#include <iostream>

int main() {
  std::cout << "String\n";
}
```
It doesn't have to be a string, it can also be emojis and other characters.
Like 🚙💨 works.
### 10/24/26
* Spent an entire 2 hours figuring out how to download unreal engine.
  * There's like 5 steps and a bug that makes it so that the download button is grayed out.
    * Found out that you also have to download twin motion to have unreal be downloadable (a visualization tool that wasn't even included in the steps).
* Official Unreal Documentation: [https://dev.epicgames.com/documentation/unreal-engine/unreal-engine-5-8-documentation](https://dev.epicgames.com/documentation/unreal-engine/unreal-engine-5-8-documentation).

Takes an entire hour to install after figuring out the steps.

### 10/25/26
* When in the editor, use wasd to move around and q and e to fly.
* R = Scale (changing the length and width
* E = Rotate along 3 different axes.
* W = Move (press w to get the interface for moving stuff.
* In the bottom left corner, there's a content drawer where you move in parts to the level.
* Details panel on the right side of the screen (after clicking a block) allows you to set the properties of an object.
* The outlier panel displays all blocks currently on the level.
* You can double click the object's picture to edit its color and physical properties (basically everything with a picture can be double clicked to change properties).
  * Base color = Color
  * Metallic = How well light reflects on it
  * Roughness = How well other objects are reflected on it. (0 = you can see what is currently facing the object).
* Holding L and clicking adds a light that is visible for both you and the player (the player doesn't see the lightbulb, they just see a patch of light).
* Holding ctrl l and moving your mouse changes the angle of the sun.
### 11/2/26
* return 0
  * The return statement is used to end a function. Returning a value indicates to the system that the code was executed successfully.
  * This part is optional.
* C++ ignores whitespace with a small exception with if statements.
  
* The 4 steps in C++
  * Code
  * Save
  * Compile
  * Execute
* To compile a file, use g++ fileName.cpp
  * It creates a machine code file called a.out
  * You can also use g++ fileName.cpp -o newFileName
    * This names the machine code filed created as newFileName
* To execute a file, use ./machineCodeFile (which is a.out unless you rename it)
### 11/3/26
* After clicking on an object, you can directly enable the physics and gravity for it.
* Also allows you to edit the mass of an object (click the checkbox).
* There's also
  * Linear Damping -- a property that slows down an object's movement over time.
  * Angular Damping -- a property that slows down an object's rotation over time.

There's tools for animating characters but it doesn't show them in the tutorial.

* The Sequencer Tool
  * Used for cinematics and cutscenes.
 
* Blueprints
  * Unreal's visual scripting language (use it alongside C++).
    * Allows logic and managing events.
    * Blueprints can be accessed in the content drawer.
    * After making a blueprint, you have to set the "Trigger" to be that blueprint (took way too long to figure this out).
### 11/4/26
(I forgot to add this so I'll add this now.)  
Comments in C++: same as every other coding language.  
Types in C++
* int -- integer numbers
* double -- floating point numbers
* char -- character
* string -- sequence of characters
* bool -- stores true or false.
  
Variable declaration and initialization are the same as Java:  
type name = value;

Single equal signs are "ASSIGN" not "EQUAL".

### 11/16/26
* Arithmetic Operators are the same as other languages.
* std::cout << varName << "\n"
  * Better than concatenation as it uses less memory and avoids segmentation faults (core dumped).
  * Basically with couts, always use << instead of +.
* `>>`
  * get from
* cin
  * Standard Input Stream
  * Pronounced "see-in" for character input.
* std::cin >> varName;
  * Passes in the (user) input into varName.
* std::string message = "text";
  * Creating a string variable called message.
  * Just string message = text; doesn't work.
* const type varName = value;
  * Can't be changed later on; stays constant and unmodifiable.
* Type conversion
  * (type) value
    * Convert value to type.
    * Going from double to int just removes the decimals without any rounding done (truncated).
* If statements are the same as any other language.
* Relational operators are the same as in any other language.

Switch Statements.
``` C++
switch (var){
   case value:
      code
      break;
   case value2:
      code 
      break;
   default:
      code
      break;
}

```
--> Add explanation later.
### 11/20/26
* Templates
  * To create a project from a template,
    * Start unreal's launcher (before entering any games) or in the main editor menu, file > new project (when in you're already in a game, top left).
   
* Samples
  * Basically just showcases more of unreal.
  * Launcher > samples
    
* ctrl hold lmb after clicking on an object moves it up and down (why would you use this).
* ctrl hold rmb after clicking on an object moves it left and right (why would you use this).

* To get back to the launcher, you have to close the editor and reopen it.
* Many more tutorials in the launcher itself (under resources and community).

* For some reason, both spaces and dashes are not allowed in the name of a project.
* Unreal gives a few base templates when creating a project, including top-down, first person, and third person.
* ...It takes 5 minutes to make a project (like after putting in a projectName, you have to wait 5 minutes for it to finish creating).
* After loading, it briefly takes up an insane amount of memory/cpu (like 96%) so it might be difficult to run with too many assets with a bad computer.
  * Drops to 40% cpu and 70% memory later and the character moves smoothly.
* Lights look really bad if used inproperly.
* The third person template is really good for what I want to make.

* Fabs (things created by other users) can be added to a project in the _epic games launcher_ (there's a rotation of free fabs every 2 weeks so just grab them).
* They're separate in the content drawer but don't function properly without proper blueprinting.
* Threw a bunch of stone golems down but they don't do anything (other than the one that's just an animation, that one just repeats the animation over and over).
* To have a proper enemy, you probably chain together several animations.
### 11/23/26
Explanation of switch Statements:

``` C++
switch (var){
   case value:
      code
      break;
   case value2:
      code 
      break;
   default:
      code
      break;
}

```
The switch keyword initializes the statement.  
The () contains the value (variable) that each case will compare.  
It must be an integral type (int, char, short, long, or enum).  
The case keyword checks if the variable matches the value that comes right after (pretty much just if X = Y).  
Runs if they match.  
The break; keyword tells the computer to exit and not run any other code or check the other cases.  
* Without break; at the end of each case, the program executes the code for the first matching case and everything that follows, including the default statement.
The default statement tells the computer what to do if none of the cases are true.

Logical operators are the same as in every other language.
* `and` can be used in place of `&&`.
* `or` can be used in place of `||`.
* `not` can be used in place of `!` (not var).
### 11/24/26
While loops are the same as in other languages.    
The escape sequences all work (\n, \t, etc).  
For loops are the same as in other languages.

Compile time errors: errors found by the compiler.  
* Syntax errors: errors that occur when you violate the rules of C++ syntax.
* Type errors: errors that occur when there are mismatches between the types declared.

Link-time errors: errors found by the linker when trying to combine object files into an executable program.  
* The program needs some function or library that it can't find.
As programs get bigger and we get more files, the linker has to do more work _linking_ all the files into a single executable file.
* Good practice to divide programs into smaller files.
* Common Types:  
  * Using a function that is undefined.
  * Using `Main` instead of `main`.

If a program has no compile-time or link-time errors, it will run.

Run-time errors: errors found by checks in a running program.  
* Occurs when we ask the computer to do something it cannot reliably do.
* Common Types:
  * Division by 0.
  * Trying to open a file that does not exist.
    
Logic errors: errors found by the programmer looking for the cause of erroneous (faulty) results.  
* The program runs successfully but doesn't produce the results we want.

Google and Stack Overflow is a programmer's best friend.

<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
