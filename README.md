# SIBOOR-V0.2-AUG
### [BOM](https://github.com/Lzhikai/SIBOOR-Voron-0.2-AUG/blob/main/SIBOOR_V0.2_AUG_BOM.md)  
### [0.2-LED-Wiring](https://github.com/Lzhikai/SIBOOR-Voron-0.2-AUG/blob/main/0.2-LED-Wiring) ：About the wiring of the sibor kit to the hot-side LED.  
### [Metalsupplements](https://github.com/Lzhikai/SIBOOR-Voron-0.2-AUG/blob/main/Metalsupplements) ： Print files not included in the CNC version.  
### [supplementary](https://github.com/Lzhikai/SIBOOR-Voron-0.2-AUG/blob/main/supplementary) ： Unlike the official installation documentation, the installation needs to be done in conjunction with the official documentation and our documentation.
<br/><img src=https://github.com/Lzhikai/SIBOOR-Voron-0.2-AUG/blob/main/0115SIBOOR%20V0.2-wiring.jpg width="600"/><br/>

Certainly! Here is the content in English, integrated into a Markdown (.md) format:

## Fixing MCU Read Error for Display Screen

If you encounter an error reading the display screen MCU, it may be due to the lack of pre-flashed firmware on the display. To address this issue, follow these optimization steps:

1. Open an SSH session and log in to the system.

2. In the terminal, enter the following commands:
   ```bash
   cd ~/klipper/
   make -j4 flash FLASH_DEVICE=0483:df11
   ```

3. After running the above command, the system may prompt you to enter a password. Enter the password: mellow.

4. Wait for the firmware to be flashed.

5. After the flashing is complete, restart the system with the following command:
   ```bash
   sudo reboot
   ```

6. Once the system restarts, the display screen should light up.

By following these steps, you should be able to resolve the issue of being unable to read the display screen MCU and ensure that the display screen has the necessary pre-flashed firmware.
