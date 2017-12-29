##Overview

1. Create a folder, e.g. hw
1. Create your code in this folder, e.g. hw/hw.cpp
1. Create a CMakeLists.txt file in this folder with the following contents:

```
cmake_minimum_required(VERSION 2.8.9)
project (hw)
add_executable(hw hw.cpp)
```

This effectively creates a *project* called "hw".

1. Now, create a subfolder under hw called, e.g. build, and change to that directory, i.e. make it the default directory.

```
mkdir build
cd build
```

1. Now, within the **build** folder, run **CMake**, passing the path to the parent directory (..) which contains CMakeLists.txt. This will generate the *build* files within the current folder, which is the **build** folder.

```
cmake ..
```

1. Finally, within the build folder, run **make**. This, at last, generates the executable file.

```
make
```

##References
The following is about the simplest, most straight-forward tutorial I've found:

http://derekmolloy.ie/hello-world-introductions-to-cmake