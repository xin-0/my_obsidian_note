
## header
```cpp

#include "header.h" // 该头文件属于当前工程
#include <header.h> // 该头文件属于外部引用，引用自其他工程、系统库等

```

自己写的用: ""
引用其他库: <>

当<>引用的不是系统库的时候，为避免编译时找不到，应在工程CMake中配置`include_directories{}`加入对应路径。

##  type

| classic        | preferred|
| :-------------- | :-------- |
| int            | int32_t  |
| unsgined int   | uint32_t |
| unsinged char  | uint8_t  |
| short          | int16_t  |
| unsigned short | uint16_t |
| long long      | int64_t  |

types in the preferred list is provided in the <stdint.h>

## variable name

### rule

- camelCase
- <type> + <name>

example:

```cpp
typedef struct_image_data{
  int32_t nFrameNo;
  int32_t nWidth;
  int32_t nHeight;
  int32_t nPixelByte;
  int8_t* pImageData;
}imageData
```

## function name

- camelCase

## software design paradigm

High cohesion & Low coupling 

variables and header files that only used or required by xxxx.c/cpp file should not be put into xxxx.h

## to avoid multiple include

```cpp
#ifdef
#define

// code

#endif

```








