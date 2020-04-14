# Change special weapon
Press the D-pad controller or press the L button together to change the special weapon.

The core code is

    580F0000 02DBDBA0
    580F1000 00000028
    580F1000 000001E0
    580F1000 00000098
    780F0000 00000064
    640F0000 00000000 000000XX

XX is the number of special you want to change.

    00 :Tenta Missiles
    01 :Ink Armor
    02 :Splat Bomb Launcher
    03 :Suction Bomb Launcher
    04 :Burst Bomb Launcher
    05 :Curling Bomb Launcher
    06 :Autobomb Launcher
    07 :Sting Ray
    08 :Inkjet
    09 :Splashdown
    0A :Ink Storm
    0B :Baller
    0C :Bubble Blower
    0D :Rain maker(We can't shoot and it's never ending.)
    10 :Tenta Missiles(doesn't work)
    11 :Booyah Bomb
    12 :Ultra Stamp
    13 :Killer Wail(We can't shoot)

#Button code

In order for us to use it freely, we need a button code.

For example,

    80004000
    580F0000 02DBDBA0
    580F1000 00000028
    580F1000 000001E0
    580F1000 00000098
    780F0000 00000064
    640F0000 00000000 00000001
    20000000

This code means changes special weapon to Ink Armor, when pushed D-pad right.

We can specify the button.
Select the number that goes into XXXXXX.

80XXXXXX

    0000001 - A
    0000002 - B
    0000004 - X
    0000008 - Y
    0000010 - Left Stick Pressed
    0000020 - Right Stick Pressed
    0000040 - L
    0000080 - R
    0000100 - ZL
    0000200 - ZR
    0000400 - Plus
    0000800 - Minus
    0001000 - Left
    0002000 - Up
    0004000 - Right
    0008000 - Down
    0010000 - Left Stick Left
    0020000 - Left Stick Up
    0040000 - Left Stick Right
    0080000 - Left Stick Down
    0100000 - Right Stick Left
    0200000 - Right Stick Up
    0400000 - Right Stick Right
    0800000 - Right Stick Down
    1000000 - SL
    2000000 - SR

Add up the numbers if you want to specify if they were pressed along with other buttons.

For example,

L + Up becomes 002040


