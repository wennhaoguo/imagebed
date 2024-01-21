# CMakeList

1. include_directories(include)

   1. in CMakeList, the current directory is where the CMakeList locates, so the include is the directory include

   2. if we don't write, the compiler gcc would search the default directories, such as

      - /usr/local

   3. catkin_INCLUDE_DIRS

      This includes the automatically generated directories such as `devel/include` where the header files are placed during the build.

   4. CMakeList tell the compiler the directories, in cpp file you use some head file. Compiler will find these headfiles during Compilation. This two path would be connected. So that you know how to write the include in cpp file.