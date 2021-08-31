# glad33core
Small library providing the glad OpenGL 33 core loader.

Besides the automatically generated glad files (https://glad.dav1d.de/#profile=core&language=c&specification=gl&loader=on&api=gl%3D3.3),
this repository provides a CMakeLists.txt to build a glad library. This allows for fetching glad into your cmake build like this:

```
# Your CMakeLists.txt...

FetchContent_Declare (
    glad
    GIT_REPOSITORY https://github.com/sreiter/glad33core
    GIT_TAG 031ed6e)

FetchContent_MakeAvailable (glad)

target_link_libraries (yourTarget glad)
```

and to include glad in a source file like this

```
// Your C/CPP/H/HPP file...

#include <glad/glad.h>
```
