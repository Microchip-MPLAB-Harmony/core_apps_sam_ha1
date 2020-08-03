[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# Title

This example application demonstrates the multi instance feature of the asynchronous mode of the USART driver.

## Description

This example uses the USART driver in asynchronous mode to communicate over two UART consoles. It echoes the characters entered by the user on the respective console.

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_sam_ha1) and then click Clone button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/driver/usart/async/usart_multi_instance/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_ha1_xpro.X | MPLABX project for [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| sam_ha1_xpro.X | [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) |
|||

- To run the demo, the following additional hardware are required:
    - [USB UART click board](https://www.mikroe.com/usb-uart-click)
    - [mikroBUS Xplained Pro board](https://www.microchip.com/developmenttools/ProductDetails/ATMBUSADAPTER-XPRO)

### Setting up [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)

- Connect the [mikroBUS Xplained Pro board](https://www.microchip.com/developmenttools/ProductDetails/ATMBUSADAPTER-XPRO) to the EXT1 header of the [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)

- Install an [USB UART click board](https://www.mikroe.com/usb-uart-click) on to the [mikroBUS Xplained Pro board](https://www.microchip.com/developmenttools/ProductDetails/ATMBUSADAPTER-XPRO)

- Connect a micro USB cable to the DEBUG port. This will enumerate a first port.

- Connect mini USB cable to the [USB UART click board](https://www.mikroe.com/usb-uart-click). This will enumerate the second port.

*Note: ATSAMHA1G16A device in SAM HA1G16A Xplained Pro board is not recommended for new design, hence replace the device with ATSAMHA1G16AB device. Connect the supported external debugger to Cortex Debug Port*

## Running the Application

1. Open the Terminal application (Ex.:Tera Term) on the computer for two COM ports.
2. Configure the serial port settings as follows:

    Baud : 115200

    Data : 8 Bits
    
    Parity : None
    
    Stop : 1 Bit
    
    Flow Control : None

3. Build and program the application using the MPLAB X IDE.

4. Type a character and observe the output on the two consoles as shown below:

5. If success the character typed echoes back and an LED toggles on each time the character is echoed.

    |![output](images/async_usart_multi_instance_console_1.png)	|
    |:--:|
    | Output on console 1 |

    |![output](images/async_usart_multi_instance_console_2.png)	|
    |:--:|
    | Output on console 2 |

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) | LED0 |
|||