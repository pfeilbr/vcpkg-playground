# how to use a package(sqlite3)

<https://github.com/Microsoft/vcpkg/blob/master/docs/examples/using-sqlite.md>

## Requirements

* cmake
* [vcpkg](https://github.com/Microsoft/vcpkg) installed

## Build and Run

```sh
cd ~/dev/vcpkg # your vcpkg install location may be different
./vcpkg install sqlite3
cd ~/projects/vcpkg-playground
mkdir using-sqlite
cd using-sqlite
touch CMakeLists.txt # populate
touch main.cpp # populate
mkdir build
cd build
cmake .. "-DCMAKE_TOOLCHAIN_FILE=/Users/brianpfeil/dev/vcpkg/scripts/buildsystems/vcpkg.cmake"
make
./main
```