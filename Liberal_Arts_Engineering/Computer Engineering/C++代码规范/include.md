```cpp

#include "header.h" // 该头文件属于当前工程
#include <header.h> // 该头文件属于外部引用，引用自其他工程、系统库等

```

自己写的用: ""
引用其他库: <>

当<>引用的不是系统库的时候，为避免编译时找不到，应在工程CMake中配置`include_directories{}`加入对应路径。