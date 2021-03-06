# Sparen's Danmakufu Standard Library

This is a library of various data structures and other utilities for use in the Touhou Danmakufu ph3 language.

### Usage

To utilize these libraries, include them using the standard Danmakufu ph3 `#include` like so:

```
#include "./stl_math.dnh"
#include "./stl_queue.dnh"
```

Each library must be included individually.

The libraries in this repository are all standalone and have no dependencies unless otherwise stated.

### Libraries

The following general libraries are provided in this distribution. These are libraries custom-made for the STL distribution.

* `stl_math.dnh` [Dependencies: None]
    - `stl_complement()`: Return the one's complement of the input as an Integer.
    - `stl_bit_not()`: Return the bitwise NOT of the input as an Integer.
    - `stl_lshift()`: Return the input left shifted n times.
    - `stl_rshift()`: Return the input right shifted n times.
    - `stl_dectobin()`: Return the input as a binary string.
    - `stl_bintodec()`: Return the input binary string as an Integer.
    - `stl_bit_and()`: Return the bitwise AND of the inputs as an Integer.
    - `stl_bit_or()`: Return the bitwise OR of the inputs as an Integer.
    - `stl_bit_xor()`: Return the bitwise XOR of the inputs as an Integer.

* `fstl_math.dnh` [Dependencies: None]
    - `fstl_bit_not()`: Return the bitwise NOT of the input as an Integer.
    - `fstl_lshift()`: Return the input left shifted n times.
    - `fstl_rshift()`: Return the input right shifted n times.
    - `fstl_bit_and()`: Return the bitwise AND of the inputs as an Integer.
    - `fstl_bit_and_arr()`: Return the bitwise AND of the values of the input array as an Integer.
    - `fstl_bit_or()`: Return the bitwise OR of the inputs as an Integer.
    - `fstl_bit_or_arr()`: Return the bitwise OR of the values of the input array as an Integer.
    - `fstl_bit_xor()`: Return the bitwise XOR of the inputs as an Integer.
    - `fstl_any_zero()`: Returns true if any of the values in the input array is 0.
    - `fstl_all_zero()`: Returns true if all of the values in the input array are 0.

The following data structure libraries are provided in this distribution. These are data structure libraries custom-made for the STL distribution.

* `stl_dict.dnh`
* `stl_queue.dnh`
* `stl_stack.dnh`

The following miscellaneous libraries are provided in this distribution. These are libraries for specific tasks that were typically made independently of the STL distribution.

* `lib_autoformat.dnh`: Provides automatic line breaking in text and text clipping functionality based on render width.
    - `autoformLineInsertionA1()`: Tokenizes the input string and outputs the same string but with spaces replaced by [r] newlines when required.
    - `autoformLineInsertionA2()`: Same as A1 but also assigns to the provided Text Object.
    - `autoformWordClipA1()`: Tokenizes the input string and outputs the same string but clipped by word to the max width.
    - `autoformWordClipA2()`: Same as A1 but also assigns to the provided Text Object.
    - `autoformCharClipA1()`: Tokenizes the input string and outputs the same string but clipped by character to the max width.
    - `autoformCharClipA2()`: Same as A1 but also assigns to the provided Text Object.

### Running Tests

Each of the unit and integration tests (*_test.dnh) are Stage scripts that can be run by Danmakufu.

If one of the assertions fails, please note so on GitHub Issues. If there are compatability issues between this library and others, please let me know so that the libraries in this distribution can be adjusted.

### Contributing

This distribution is primarily maintained by myself. I welcome all suggestions and bug reports. If you would like to make a pull request, please feel free.
