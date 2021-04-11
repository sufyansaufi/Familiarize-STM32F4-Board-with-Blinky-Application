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

* A new project name LED_BLINKING is created using STM32CubeIDE and STM32CubeMX.
* Board is selected from the board selector in CubeMX so that it can pre-populate all pins that are connected on the board.
* The LED that will be used for this project is determined which is at PA5 and declared it as GPIO Output and the user label is LD2[green_Led].
* Code is generated after all configuration is done and some of the driver will require update to support the board.
* In the main loop, HAL functions are called to make the desired LED to blink:
* **HAL_Init();** //Reset of all peripherals, Initializes the Flash interface and the Systick.
* **SystemClock_Config()**; //called the SystemClock function to configure the system clock
* /* Initialize all configured peripherals */
  **MX_GPIO_Init();**
  **MX_USART2_UART_Init()**;
* **HAL_GPIO_TogglePin(GPIOA, GPIO_PIN_5);** //oggle the LED
* **HAL_Delay(500);** // Delay 
* *500ms* is used to make the LED blink every 1 second
* The code is pushed to the board using the STSWLink.
* Reset button is pressed to make the board execute the blinky code.
