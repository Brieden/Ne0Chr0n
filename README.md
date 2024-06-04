# Ne0Chr0n
Keychron Q2 Pro QMK with Neo2


## Description
- **The Keychron Q2 Pro** is a high-quality, customizable mechanical keyboard. It supports various key switches and is compatible with QMK firmware.
- **QMK** (Quantum Mechanical Keyboard) is a powerful open-source firmware for keyboards. It allows users to customize keymaps, macros, and functions to fit their needs.
- **Neo2** is an ergonomic keyboard layout optimized for the German language. It focuses on minimizing finger movement and increasing typing speed.

## Requirements
- [QMK Firmware](https://github.com/qmk/qmk_firmware/tree/master/keyboards/keychron/q2)
- [Keychron Q2 Pro Keyboard](https://www.keychron.com/products/keychron-q2-pro-qmk-via-wireless-custom-mechanical-keyboard)
- [Neo2 Layout](https://neo-layout.org/)


## Installation
1. Setting Up Your [QMK Environment](https://docs.qmk.fm/newbs_getting_started)\
   But finish the steps with a specific QMK repo:
   ```sh
   qmk setup Keychron/qmk_firmware.git -b bluetooth_playground
    ```
2. Clone the Ne0Chr0n repository into the appropriate directory of the QMK structure:
    ```sh
    cd qmk_firmware/keyboards/keychron/q2_pro/ansi_encoder/keymaps
    git clone https://github.com/Brieden/Ne0Chr0n.git
    ```
3. Compile the firmware:
    ```sh
    qmk compile -kb keychron/q2/ansi_encoder -km Ne0Chr0n
    ```
4. Flash the firmware to your Keychron Q2 Pro:
    ```sh
    qmk flash -kb keychron/q2/ansi_encoder -km Ne0Chr0n
    ```

## Acknowledgements

This project was inspired by the work from Hannes Leutloff to bring Neo2 with QMK to the ErgoDox [qmk-neo2](https://github.com/yeldiRium/qmk-neo2/blob/master/keymap.c)