# CFexpress PCIe Hat for Raspberry Pi 5
Welcome to the GitHub repository for the open-source CFexpress (CFE) PCIe Hat designed specifically for the Raspberry Pi 5. This project aims to enhance the Raspberry Pi 5 by adding the ability to interface with CFexpress Type B cards directly, enabling high-speed data transfer and storage solutions.
![](https://github.com/will127534/RPI5-CFE-Hat/blob/images/_DSC4473-3.jpg)

## Features
* CFexpress Type B Card slot: Directly connect a CFexpress Type B card to your Raspberry Pi 5 for high-speed data storage and transfer.
* Automated Card Mounting: Utilizes a CH32V003 MCU for I2C to GPIO control, enabling the automated mounting and unmounting of the CFexpress card with the press of an eject button.
* QWIIC Hub: Includes a simple QWIIC hub that provides four additional QWIIC ports, allowing for easy expansion and connectivity with other QWIIC-compatible devices.
* Flexible Mounting Options: Designed to be mounted either on the top or the bottom of the Raspberry Pi 5. When mounted on top, the I2C connection is made directly from the GPIO header on the Raspberry Pi 5. For bottom mounting, the QWIIC port is used to connect and enable the auto-mount script.

## Notes
* Automounting feature requires I2C connection from either QWIIC port or RPI GPIO
* The board does not support hot-unplug even with the auto-mount script, so you will need to press the eject button to signal unmount request
* Gerber and CPL file for JLCPCB is under /Gerber
* Bom for interactive bom html [provided by InteractiveHtmlBom
](https://github.com/openscopeproject/InteractiveHtmlBom) and JLCPCB BOM under /bom
* Source Code for CH32V003 based I2C to GPIO and Python code on RPI under /software

## Support
For questions, issues, or suggestions, please open an issue in the [GitHub repository](https://github.com/will127534/RPI5-CFE-Hat/issues)  
Also see [Quick Start Guide](https://github.com/will127534/RPI5-CFE-Hat/wiki/RPI5-CFE-Hat-Quick-Start-Guide)

## License
This project is licensed under the MIT License - see the LICENSE file for details.
