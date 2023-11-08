# MAIN-IN-RAIN-animation-using-Turbo-C
The provided code is a C program that uses the Turbo C graphics library to create a simple animation of rain, a hut, a person with an umbrella, and a rainbow. Here is a brief overview of the different components and functions in the code:

1. **Header Files:** The program includes several header files, including `conio.h`, `graphics.h`, and `stdio.h`. These headers are used for console I/O and graphics operations.

2. **Macros and Global Variables:**
   - `ScreenWidth` and `ScreenHeight` are defined using the `getmaxx()` and `getmaxy()` functions to get the screen dimensions.
   - `GroundY` is set to 75% of the screen height, representing the ground level.
   - `ldisp` is a variable used to control the movement of the umbrella.

3. **hut():** This function draws a simple hut with rectangles and lines. It uses the `rectangle()` function to draw the hut's walls and `line()` functions to draw the roof.

4. **DrawManAndUmbrella():** This function draws a person with an umbrella. It uses circles and lines to create the person and the umbrella. The `x` and `ldisp` parameters control the position and movement of the person and the umbrella.

5. **Rain():** This function generates raindrops on the screen. It uses random positions to draw lines representing raindrops. Raindrops are not drawn below the ground level.

6. **rainbow():** This function draws a rainbow on the screen using arcs of various colors. It also animates the appearance of the rainbow.

7. **main():** The `main()` function initializes the graphics mode using `initgraph()`. It then enters a loop that continues until a key is pressed (using `kbhit()`). Within the loop, it continuously updates the rain, the person with the umbrella, and clears the screen to create the animation.

   When a key is pressed, it stops the rain animation and calls the `rainbow()` function to display the rainbow.

Please note that this code is specifically written for the Turbo C graphics library, which is a DOS-based graphics library and may not work on modern systems without an emulator or a DOS environment. Additionally, modern C/C++ compilers and IDEs typically have better graphics libraries and do not rely on Turbo C.
