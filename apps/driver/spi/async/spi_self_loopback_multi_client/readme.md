[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# Title

This example demonstrates the multi client feature of the SPI driver by performing self-loop back with two clients connected on the same SPI bus

## Description

- This example demonstrates the multi client feature of the SPI driver by reading and writing data with two clients that are connected on the same SPI bus

- It uses the request (write and read request) queuing feature of the asynchronous driver and does not waste CPU bandwidth in waiting for previous request completion

- The example also demonstrates how to setup two different client transfers at different baud rates

- This example performs self loop back only once after a power on reset

- Success is indicated when a successful self loop back is reported by both the clients

- After the loop back test is complete, the application remains in the idle state


## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_sam_ha1) and then click Clone button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/driver/spi/async/spi_self_loopback_multi_client/firmware** .

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

### Setting up [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)

- Use jumper wire to Connect "Pin 16 of EXT1 header" to "Pin 17 of EXT1 header"

    - SPI0 MOSI signal is mapped to PA04 that is routed to "Pin 16 of EXT1 header"

    - SPI0 MISO signal is mapped to PA11 that is routed to "Pin 17 of EXT1 header"

- Connect the Debug USB port on the board to the computer using a micro USB cable

*Note: ATSAMHA1G16A device in SAM HA1G16A Xplained Pro board is not recommended for new design, hence replace the device with ATSAMHA1G16AB device. Connect the supported external debugger to Cortex Debug Port*

## Running the Application

1. Build and program the application using its IDE
2. The LED is turned ON on Success

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) | LED0 |
|||