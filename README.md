# STM32FR11RE-Peripheral-Project

## Overview
This is a bare-metal STM32 project demonstrating:
- LED control on PA5
- Button input using EXTI on PC13
- USART2 serial communication (TX)
- TIM2 timer interrupts

## Features
- LED toggles every 1 second using TIM2 interrupt
- LED toggles on button press
- Button press sends character 'c' over USART2
- Fully interrupt-driven design

## Hardware
- STM32F411RE Nucleo Board
- Built-in LED (PA5)
- User button (PC13)

## Notes
- All peripheral configuration is done using direct register access (no HAL)
- Baud rate: 9600 bps, 16 MHz clock
- Prescaler and ARR set for 1-second timer overflow
