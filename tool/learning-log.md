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

<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
