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

The following data structure libraries are provided in this distribution. These are data structure libraries custom-made for the STL distribution.

* `stl_queue.dnh`
* `stl_stack.dnh`

The following miscellaneous libraries are provided in this distribution. These are libraries for specific tasks that were typically made independently of the STL distribution.

* `lib_autoformat.dnh`: Provides automatic line breaking in text based on render width.

### Running Tests

Each of the unit and integration tests (*_test.dnh) are Stage scripts that can be run by Danmakufu.

If one of the assertions fails, please note so on GitHub Issues. If there are compatability issues between this library and others, please let me know so that the libraries in this distribution can be adjusted.

### Contributing

This distribution is primarily maintained by myself. I welcome all suggestions and bug reports. If you would like to make a pull request, please feel free.
