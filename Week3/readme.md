# Home work week 3

##  Intro

I have made an attempt to make the orange LED on the STM32F411E-DISCO board blink using interrupts. I haven't gotten to setup a timer to make debouncing.

## Build environment

As I am completely new to embedded and STM32 I have used STM32CubeIDE because there are many tutorials on how to use it. When I get more used to the HAL, I think I will go with VS Code instead, because STM32CubeIDE also forces a lot upon you.

## Questions from the assigment

### Can you step through the code to see what each line does?

Yes, using the ST-Link through STM32CubeIDE this is very easy to do.

### What are the hardware registers that cause the LED to turn on and off?

If I go into GPIO_TypeDef I believe I need to look at ODR, which shows this /*!< GPIO port output data register,        Address offset: 0x14      */

### What are the registers that you read in order to find out the state of the button?

If I look into the reference manual in section 8.4.5 it look like the address offset i 0x10.

### Can you read the register directly and see the button change in a debugger or by printing out thes value of the memory at the register’s address?

Most likely, but I haven't managed to try it.