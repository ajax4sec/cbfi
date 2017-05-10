# Coverage Based Fault Injection
Coverage based fault injection.
Added python wrapper


# Compiling coreutils-8.27 with gcov
1. Unzip/uncompress coreutils-8.27.tar.xz into a folder
2. Rename folder to `coreutils`
3. `cd coreutils`
4. `./configure CFLAGS="-g --coverage -rdynamic"`
5. `make`
7. Coreutils executables will be in `/absolute/path/to/some/folder/src`
8. `rm *.gcda` before each run of a coreutils executable
9. `gcov -i executable.c` to generate gcov of a coreutil such as cat, ls etc
