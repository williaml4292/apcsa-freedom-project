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
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
