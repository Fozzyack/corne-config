# Corne Keyboard Configuration

ZMK firmware configuration for a Corne (3x6+3) split keyboard.

## Layers

### Default Layer
Standard QWERTY layout with home row modifiers.
- Hold left thumb middle key for Lower layer
- Hold left thumb inner key for Raise layer

### Lower Layer (Doom)
Numbers, brackets, and navigation.
- Number row (1-0)
- Arrow keys on right hand home row
- Parentheses and angle brackets
- Access Utils layer with right pinky

### Raise Layer (Spark)
Symbols and special characters for coding.
- Symbols row (!@#$%^&*+=)
- Brackets and braces
- Caps Lock and Caps Word support

### Utils Layer (Fkey)
Function keys, Bluetooth, and media controls.
- F1-F12 function keys
- Bluetooth pairing (BT0-BT3) and clear
- Media controls (mute, volume)
- External power toggle

## Building

This configuration uses GitHub Actions for automated builds. Firmware files are generated on every commit.

## Flashing

1. Download the firmware from GitHub Actions artifacts
2. Connect keyboard via USB
3. Double-tap reset button to enter bootloader mode
4. Copy `.uf2` file to the mounted drive
