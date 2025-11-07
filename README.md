# Corne Keyboard Configuration

ZMK firmware configuration for a Corne (3x6+3) split keyboard.

## Layers

### Default Layer
Standard QWERTY layout with home row modifiers.
```
┌──────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬──────┐
│ TAB  │  Q  │  W  │  E  │  R  │  T  │   │  Y  │  U  │  I  │  O  │  P  │ BSPC │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ CTRL │  A  │  S  │  D  │  F  │  G  │   │  H  │  J  │  K  │  L  │  ;  │  '   │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ SHFT │  Z  │  X  │  C  │  V  │  B  │   │  N  │  M  │  ,  │  .  │  /  │ ESC  │
└──────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴──────┘
                   │ GUI │ LWR │ SPC │   │ ENT │ RSE │ ALT │
                   └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Lower Layer (Doom)
Numbers, brackets, and navigation.
```
┌──────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬──────┐
│ TAB  │  1  │  2  │  3  │  4  │  5  │   │  6  │  7  │  8  │  9  │  0  │ DEL  │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ TRNS │TRNS │  <  │  (  │  )  │  >  │   │ LFT │ DWN │ UP  │ RGT │TRNS │ TRNS │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ SHFT │TRNS │TRNS │TRNS │  <  │  >  │   │TRNS │TRNS │TRNS │TRNS │TRNS │ MO 3 │
└──────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴──────┘
                   │ GUI │TRNS │TRNS │   │ ENT │ SPC │RGUI │
                   └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Raise Layer (Spark)
Symbols and special characters for coding.
```
┌──────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬──────┐
│ TAB  │  !  │  @  │  #  │  $  │  %  │   │  ^  │  &  │  *  │  +  │  =  │ BSPC │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ ESC  │TRNS │TRNS │  =  │  -  │  :  │   │  [  │  {  │  }  │  ]  │  \  │  `   │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ SHFT │TRNS │TRNS │  +  │  _  │  "  │   │  <  │  (  │  )  │  >  │  |  │  ~   │
└──────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴──────┘
                   │ GUI │CAPS │TRNS │   │ ESC │ SPC │CPSWD│
                   └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Utils Layer (Fkey)
Function keys, Bluetooth, and media controls.
```
┌──────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬──────┐
│ EPWR │ F1  │ F2  │ F3  │ F4  │ F5  │   │ F6  │ F7  │ F8  │ F9  │ F10 │ F11  │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│BTCLR │ BT0 │ BT1 │ BT2 │ BT3 │  G  │   │  H  │  J  │  K  │  L  │  ;  │ F12  │
├──────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼──────┤
│ MUTE │ VOL-│ VOL+│  C  │  V  │  B  │   │  N  │  M  │  ,  │  .  │  /  │ ESC  │
└──────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴──────┘
                   │ GUI │TRNS │TRNS │   │ ENT │ SPC │ ALT │
                   └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

## Building

This configuration uses GitHub Actions for automated builds. Firmware files are generated on every commit.

## Flashing

1. Download the firmware from GitHub Actions artifacts
2. Connect keyboard via USB
3. Double-tap reset button to enter bootloader mode
4. Copy `.uf2` file to the mounted drive
