Data buffer transmission/reception between STM32WB55RG and CY15B108QI via SPI using DMA.  
Board: P-NUCLEO-WB55 (embeds a STM32WB55RG device)  
CLK Pin: PA5 (CN10, pin 11)  
MISO Pin: PA6 (CN10, pin 13)  
MOSI Pin: PA7 (CN10, pin 15)  
CS Pin: PA4 (pin D10)   

 _________________________                       __________________________   
|           ______________|                      |______________           |  
|          |SPI1          |                      |          SPI1|          |   
|          |              |                      |              |          |   
|          |    CLK(PA.05)|______________________|SCK           |          |   
|          |              |                      |              |          |   
|          |   MISO(PA.06)|______________________|SDO           |          |   
|          |              |                      |              |          |   
|          |   MOSI(PA.07)|______________________|SDI           |          |   
|          |              |                      |              |          |  
|          |     CS(PA.04)|______________________|CS            |          |   
|          |______________|                      |______________|          |   
|                         |                      |                         |   
|                      3V3|______________________|3V3                      |   
|                         |                      |                         |  
|                      GND|______________________|GND                      |   
|                         |                      |                         |   
|_STM32WBxx Master________|                      |_external FRAM___________|  