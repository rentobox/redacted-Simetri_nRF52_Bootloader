# Simetri_nRF52_Bootloader

This repo contains the custom SIMETRI .hex file that can be used to flash bootloader onto nRF52833 board.

## Prerequiste:
- Make sure board being used is cleared.
- Must have nRF Connect for Desktop installed.
- Download simetri52833_bootloader-0.9.2-12-ga48e944-dirty_s140_7.3.0.hex
- Open Git Bash.

## To flash onto board:
1. Make sure board is connected on the left side for flashing.
2. In Git Bash, run:
``` cd downloads ```
3. Next, run:
``` nrfjprog --program simetri52833_bootloader-0.9.2-12-ga48e944-dirty_s140_7.3.0.hex --chiperase --reset ```
4. Done

## What should happen:
LED1 should be rapidly blinking. This indicates that the bootloader has been updated.  Once it is plugged into the nRF USB slot, LED1 will turn on and off slowly, indicating it is in bootloader mode and is ready to have code flashed onto it.

Once you flash something on to it, it will be saved on. If you double click the reboot button, it will put the board back into bootloader mode and vice versa.

# Full Repo here: 
[Simetri_nRF52_Bootloader](https://github.com/rentobox/Simetri_nRF52_Bootloader) 
