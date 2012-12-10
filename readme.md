This is a fork of PJRC's [PS2Keyboard library](http://www.pjrc.com/teensy/td_libs_PS2Keyboard.html) (v2.3).
It was made to work with the Arduino Leonardo via some additional pin definitions.

Specifically, in PS2Keyboard.h, the following was added:

```
#elif defined(__AVR_ATmega32U4__)
#define CORE_INT0_PIN 3
#define CORE_INT1_PIN 2
#define CORE_INT2_PIN 0
#define CORE_INT3_PIN 1
```

This uses the additional interrupt pins (`INT0-3`) available on the Leonardo.

Hopefully this will soon be incorporated into the PJRC-hosted lib.


### License
inherited from the original:

```
GNU Lesser General Public License v2.1 or later
Copyright (c) 2007 Free Software Foundation
```
