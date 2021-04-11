# Familiarize-STM32F4-Board-with-Blinky-Application

This is the first project done to familiarize with STM development environment. 

**Youtube Video**

<a href="http://www.youtube.com/watch?feature=player_embedded&v=6JYLMo7ZYY4
" target="_blank"><img src="http://img.youtube.com/vi/6JYLMo7ZYY4/0.jpg" 
alt="Project Milestone 1" width="240" height="180" border="10" /></a>

**Development kit:**
1. STM32CubeMX
2. STM32CubeIDE

**Instruction**

* A new project is created using STM32CubeMX.
* Board is selected from the board selector in CubeMX so that it can pre-populate all pins that are connected on the board.
* The LED that will be used for this project is determined.
* The LED name is changed to be *pin_name* for easier identification.
* Code is generated after all configuration is done. 
* In the main loop, HAL functions are called to make the desired LED to blink
* **HAL_GPIO_TOGGLE**
* **HAL_Delay**
* *500ms* is used to make the LED blink every 1 second
* The code is pushed to the board.
* Reset button is pressed to make the board execute the blinky code.
