1. What GPIO port does the built-in LED on the Blue Pill PCB use?
Specify the libopencm3 macro name for the port.

- Port C , GPIOC

2. What GPIO PIN does the built-in LED on the Blue Pill PCB use? Specify libopencm3 macro name.

- Pin 13 , GPIO13

3. What level is required to turn the built-in LED on for the Blue Pill PCB?

- PC13 should be pulled down -> PC13 = 0 (GND in terms of electric voltage)

4. What are two factors affecting the chosen loop count in a programmed delay in non-multi-tasking environments?

- CPU clock cycle and the fetch time form memory

5. Why are programmed delays not used in a multi-tasking environment?

- Multi tasking environments have context switching and delays would interfere or be interfered with by that.

6. What three factors affect instruction timing?

- CPU clock cycles, instruction fetch source and the context switching

7. What are three modes of an input GPIO port?

- PULL_UP_DOWN, Analog Input, Floating

8. Do the weak pull-up and pull-down resistors participate in an analog input?

- No, only in the digital input

9. When is the Schmitt trigger enabled for input ports?

- For digital input

10. Do the weak pull-up and pull-down resistors participate for output GPIO ports?

- Yes

11. When configuring a USART TX (transmit) output for push/pull operation, which specialization macro shoud be used?

- GPIO_CNF_OUTPUT_PUSHPULL

12. When configuring a pin for LED use, which GPIO mode macro is preferredfor low EMI?

- GPIO_MODE_OUTPUT_2_MHZ
