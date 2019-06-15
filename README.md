# Lee Dohm's Keyboard Firmware

This is the firmware definition for my keyboards:

* [Ergodox EZ Shine][ergodox] with Cherry MX Blue keyswitches
* [Planck EZ Glow][planck] with Cherry MX Brown keyswitches

The firmware for both was built using the [ZSA Graphical Configurator][configurator].

[configurator]: https://configure.ergodox-ez.com/layouts/default/latest/0
[ergodox]: https://ergodox-ez.com/
[planck]: https://ergodox-ez.com/pages/planck

## Ergodox Layout

See [the PDF][ergodox-pdf] for the full layout, including all layers. Or [view on the configurator][ergodox-layout] to base your own layout on mine.

[ergodox-layout]: https://configure.ergodox-ez.com/layouts/bvZRp/latest/0
[ergodox-pdf]: ./keyboard-layout.pdf

### Features

Each layer has been customized with a background shine to indicate which layer the keyboard is on.

#### Layer 0 &mdash; Dvorak &mdash; No shine

This is designed as a fairly standard typing layout. The primary goal was to move the keys as little as possible from their typical locations on a standard Dvorak keyboard layout to minimize the errors that would occur when forced to use a standard keyboard, such as on a laptop in meetings.

**Notes:**

* <kbd>Esc</kbd> is placed to the right of <kbd>5</kbd> to make it easily accessible and to allow the <kbd>\`</kbd> to remain in its standard position to the left of <kbd>1</kbd>
* <kbd>\\</kbd> was placed to the left of <kbd>A</kbd> because I don't use <kbd>Caps Lock</kbd> and it is fairly commonly used in programming, so I wanted it on one of the two main key clusters
* <kbd>Space</kbd> is placed in the primary location on the right thumb cluster since, like most touch typists, I was trained to use only my right thumb to press the space bar
* <kbd>Enter</kbd> is placed in the secondary location on the right thumb cluster so that <kbd>-</kbd> can remain to the right of <kbd>S</kbd>
* <kbd>Backspace</kbd> and <kbd>Delete</kbd> are in the primary and secondary locations on the left thumb cluster to keep them convenient and it makes a kind of sense that they oppose <kbd>Space</kbd> and <kbd>Enter</kbd>
* <kbd>Volume Up</kbd>, <kbd>Volume Down</kbd>, <kbd>Mute</kbd>, and <kbd>Play</kbd> are on the right thumb cluster
* <kbd>Home</kbd>, <kbd>End</kbd>, <kbd>Page Up</kbd>, and <kbd>Page Down</kbd> are located on the left thumb cluster so that they are available because some applications explicitly use them
* The two <kbd>Hyper</kbd> modifiers are a combination of <kbd>Shift</kbd>, <kbd>Ctrl</kbd>, <kbd>Option</kbd>, and <kbd>Cmd</kbd>. They are designed to create OS-wide key combinations. I use them for things like:
    * <kbd>Hyper+B</kbd> to launch my browser
    * <kbd>Hyper+T</kbd> to launch my terminal
    * <kbd>Hyper+E</kbd> to launch my text editor
    * <kbd>Hyper+Space</kbd> to launch Alfred

#### Layer 1 &mdash; Arrows &mdash; Red shine

The intent of this layer is to give easy access to the standard macOS keyboard navigation combinations, specifically the <kbd>Shift</kbd>, <kbd>Option</kbd>, and <kbd>Cmd</kbd> modifiers and the four arrow keys. <kbd>Ctrl</kbd> is not used in keyboard navigation on macOS, so it doesn't have a special place on this layer.

**Notes:**

* Activating this layer is achieved by holding down either bottom vertical long key in the main key cluster on either hand
* macOS keyboard navigation is achieved with the fingers of the right hand on the home row in a WASD-style pattern and the fingers of the left hand moved to the bottom right of the main key cluster so the index finger is on the layer shift key and the other three fingers are on <kbd>Cmd</kbd>, <kbd>Option</kbd>, and <kbd>Shift</kbd>. This allows the formation of all cursor navigation combinations, using combinations of <kbd>Cmd</kbd>, <kbd>Option</kbd>, and the arrow keys, and all navigation with selection combinations by including <kbd>Shift</kbd>
* This layer also has video brightness controls in the same locations as the <kbd>Volume Up</kbd> and <kbd>Volume Down</kbd> keys in Layer 0
* This layer also includes the Ergodox EZ Shine LED controls

#### Layer 2 &mdash; Numeric keypad &mdash; Green shine

The design here is to center the numeric keypad on the middle finger of the right hand, just as it would be for touch-typing numeric entry on a standard keyboard.

**Notes:**

* Activating this layer is by toggle using the key to the left of <kbd>6</kbd>
* Because this layer is rarely used and only by the right hand, I placed <kbd>Reset</kbd> on this layer in the upper-left corner of the main key cluster of the left hand. <kbd>Reset</kbd> puts the keyboard into bootloader mode so that a new firmware can be flashed without having to find a paperclip and trigger the hardware button.

#### Layer 3 &mdash; QWERTY layout &mdash; Blue shine

This layer simply provides QWERTY-compatibility in those situations where I need the keys to be in their standard locations. This is typically for video games.

**Notes:**

* Activating this layer is by toggle using the key to the right of <kbd>5</kbd> on Layer 1. This can be toggled quickly by using the left thumb on the Layer 1 modifier key and then the left index finger on the Layer 3 toggle

#### Layer 4 &mdash; QWERTY function keys &mdash; Magenta shine

This layer allows access to standard F-keys (and `PrintScr`) for games that use them.

**Notes:**

* Activating this layer is achieved by holding down the lower-left-most key on the left hand when already in QWERTY mode on Layer 3. Release it to return to Layer 3.

## Planck Layout

View the layout on [the configurator][planck-layout]. I just got the thing, so the layout is going to be in significant flux for a while. When things settle down, I'll get around to documenting it like I did for the Ergodox.

[planck-layout]: https://configure.ergodox-ez.com/planck-ez/layouts/yo0z0/latest/0

## Installation

Download the [flashing tool](https://ergodox-ez.com/pages/wally?mc_cid=f143adc401&mc_eid=9c22d0ce78) from the Ergodox EZ website and use the `*.hex` or `*.bin` file to update the firmware.

* [Test the new firmware](http://www.keyboardtester.com/tester.html)
