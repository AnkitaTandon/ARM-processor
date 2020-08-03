# ARM-processor 
 Assembly Language Programming to program ARM processor for beginners by a beginner.
 
## Installation
To run ARM programs [download](https://drive.google.com/file/d/1D2ThQHlwVm-AKi4Ew58r6yp_oblK2fqs/view?usp=sharing) **Keil uVision** software in any drive say _ABC_

Learn how to use *Keil Software* from [here](https://www.youtube.com/watch?v=ED2wdbd6S68)

## Holds

#### Assembly lang (s/w)
1. Bubble Sort
2. Arithematic Operations: choose an option to find the sum, difference, product or quotient 
3. Fibonicci series
4. nCr 
5. Arithematic op. in **float**: sum, difference, product, square, cube

#### C lang (h/w)
1. Sine wave
2. Triangular wave
3. 7 segment display
4. Stepper Motor
5. UART: to learn the details, click [here](https://drive.google.com/file/d/1yJnENCeT2e_TFNJ5Ksa7yWCwCQfuObPv/view)!
The pdf on UART is [here](https://drive.google.com/open?id=13xdDeWjQd2ubohxqKbpDWhhpAtUOZoYl&authuser=0)

## Setup
 - Open the Keil Application> Project> New project and then create a folder

 - **if** dealing with _floating point (FPU)_
      - Under *select a device for target 1* dialogue box> search and select `STM32F401RE` cortex M4 for FPU since cortex M3 doesn't support FPU (to add .asm startup file)
      -In the file *startup_stm32f401xx.s* comment the lines 183 and 184 and save it. 
        (In ARM we use `;` to comment a line)
      - Right click on `source group1`> Add existing item to the group> _ABC_ drive> look for your ARM software folder> startup> ST> STM32F4xx> system_stm32f4xx> `ADD` 
        (to add C startup file)
  - **else** for cortex M3 operations
     - Select a device for target 1> `NXP`> `LPC1768`> OK> Add the startup file to the folder by clicking on `YES` (to add .asm startup file)
     - Right click on `source group1`> Add existing item to the group> _ABC_ drive> look for your ARM software folder> startup> NXP> LPC17XX> `Add` (to add C startup file)

 - Make sure you have 2 _existing files_, one with `.s` and the other with `.c`  
 - **if** coding in assemply lang
     - Right click on `source group1`> new item to the group> `asm.file`> Enter filename> `ADD`
  - **else if** coding in C lang
     - Right click on `source group1`> new item to the group> `c.file`> Enter filename> `ADD`

## Working
 - Type or [download](https://github.com/AnkitaTandon/ARM-processor/tree/master/src) and paste the code in the new file> save it.
 - Click on `build` or `F1` button to check for errors.
 - If it shows "no error no warning" at the comment section then click on `debug`> `OK`
 - Enter the value(s) in the memory block if required. 
 - Click `StepIn` to notice the execution of the program step by step.
 - To go back> click on `debug` again.
 
 Common Issue while deploying the code: Click on `StepOut` if stuck in repeating loop

 Thank me later ;) 
  - If you ever encounter an anonymous error, copy the entire error statement and paste it on web server. I'm sure _Stack Overflow_ will help you out.  
