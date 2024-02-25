## Size-bounded string copying and concatenation

### size_t strlcpy(char *dst, const char *src, size_t size);
This function copies up to _size - 1_ bytes of src into dst and returns src's length. In other words, it writes _size_ bytes in dst: the first _size - 1_ bytes of src and a null character ('\0') at the end. You can find this function in the [string.h](https://www.tutorialspoint.com/c_standard_library/string_h.htm) header.

Examples:
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;INPUT&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; | &emsp;&emsp;&nbsp;&nbsp;OUTPUT&emsp;&nbsp;&emsp;&nbsp;&nbsp; |
|:------------------------------------:|:------:|

| dst | src | size | rvalue | new dst |
|:---:|:---:|:---:|:---:|:---:|
| "This is dst" | "Src is this" | 4 | 11 | "Src" |
