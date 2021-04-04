# Familiarize-STM32F4-Board-with-Blinky-Appplication

This is the first project done to familiarize with STM development environment. 

Board used:

Development kit:
1. STM32CubeMX
2. STM32CubeIDE

###### Setting up the board

* A new project is created using STM32CubeMX.
* Board is selected from the board selector in CubeMX so that it can pre-populate all pins that are connected on the board.

    **image**

* The LED that will be used for this project is determined (*pin*).
* The LED name is changed to be *pin_name* for easier identification.
* Code is generated after all configuration is done. 
* In the main loop, HAL functions are called to make the desired LED to blink
* **HAL_GPIO_TOGGLE**
* **HAL_Delay**
* *500ms* is used to make the LED blink every 1 second
* The code is pushed to the board.
* Reset button is pressed to make the board execute the blinky code.
