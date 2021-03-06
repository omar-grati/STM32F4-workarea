/**
  @page FSMC_SRAM SRAM memory basic functionalities use example
  
  @verbatim
  ******************* (C) COPYRIGHT 2013 STMicroelectronics ********************
  * @file    FSMC/FSMC_SRAM/readme.txt 
  * @author  MCD Application Team
  * @version V1.1.0
  * @date    18-January-2013
  * @brief   Description of the FSMC SRAM example.
  ******************************************************************************
  *
  * Licensed under MCD-ST Liberty SW License Agreement V2, (the "License");
  * You may not use this file except in compliance with the License.
  * You may obtain a copy of the License at:
  *
  *        http://www.st.com/software_license_agreement_liberty_v2
  *
  * Unless required by applicable law or agreed to in writing, software 
  * distributed under the License is distributed on an "AS IS" BASIS, 
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  ******************************************************************************
  @endverbatim
 
@par Example Description 

  This example shows how to configure the FSMC to drive the SRAM memory mounted 
  on STM3240_41_G_EVAL or STM32437I_EVAL boards. It uses an associate driver 
  developed to interface with the indicated SRAM device.
 
  After initializing the device, user can perform read/write operations on it. 
  A data buffer is written to the SRAM memory, then read back and checked to verify 
  its correctness.
  
  If the data is read correctly from SRAM, the LED1 is on, otherwise the LED2 is on.
  
@par Directory contents
                       
 - FSMC/FSMC_SRAM/system_stm32f4xx.c          STM32F4xx system clock configuration file 
 - FSMC/FSMC_SRAM/stm32f4xx_conf.h            Library Configuration file
 - FSMC/FSMC_SRAM/stm32f4xx_it.c              Interrupt handlers
 - FSMC/FSMC_SRAM/stm32f4xx_it.h              Header for stm32f4xx_it.c
 - FSMC/FSMC_SRAM/main.h                      Header for main.c module 
 - FSMC/FSMC_SRAM/main.c                      Main program

@note The "system_stm32f4xx.c" is generated by an automatic clock configuration 
       tool and can be easily customized to your own configuration. 
       To select different clock setup, use the "STM32F4xx_Clock_Configuration_V1.1.0.xls" 
       provided with the AN3988 package available on <a href="http://www.st.com/internet/mcu/family/141.jsp">  ST Microcontrollers </a>

      
@par Hardware and Software environment 

  - This example runs on STM32F40xx/STM32F41xx, STM32F427x/STM32F437x Devices.
    
  - This example has been tested with STMicroelectronics STM324xG-EVAL (STM32F40xx/
    STM32F41xx Devices) and STM32437I-EVAL (STM32F427x/STM32F437x Devices) evaluation 
    boards and can be easily tailored to any other supported device and development 
    board.

@par How to use it ? 

 In order to make the program work, you must do the following :
 - Copy all source files from this example folder to the template folder under
   Project\STM32F4xx_StdPeriph_Templates
 - Open your preferred toolchain 
 - Add the following file in the project source list:
   - STM324xG_EVAL: 
     Utilities\STM32_EVAL\STM324xG_EVAL\stm324xg_eval_fsmc_sram.c
           
   - STM324x7I_EVAL: 
     Utilities\STM32_EVAL\STM324x7I_EVAL\stm324x7i_eval_fsmc_sram.c
 - Rebuild all files and load your image into target memory
 - Run the example

 * <h3><center>&copy; COPYRIGHT STMicroelectronics</center></h3>
 */
