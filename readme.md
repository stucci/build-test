g++
```shell
g++ hello.cpp -o hello.o
```

make
```shell
sudo apt install make
```
```shell
make
./hello.o
make clean
```

cmake
```shell
sudo apt install cmake
```
```shell
mkdir build
cd build
cmake ..
make
./main.o
make clean
```

cmake on windows
* install cmake
  [Download | CMake](https://cmake.org/download/)
```powershell
mkdir build_win
cd build_win
cmake -G "Visual Studio 16 2019" -A x64 ..
msbuild hello.sln
.\Debug\main.o.exe
msbuild hello.sln -t:clean
```

bazel
* install bazel
  [Installing Bazel on Windows - Bazel](https://docs.bazel.build/versions/master/install-windows.html)
```powershell
bazel build //main:hello-bazel
.\bazel-bin\main\hello-bazel.exe
```
ref. [Build Tutorial - C++ - Bazel](https://docs.bazel.build/versions/master/tutorial/cpp.html)

gdb
```shell
sudo apt install gdb
```
```shell
g++ hello.cpp -g
gdb a.out
# break main
b main
# run
r
# next
n
# print a
p a
# info locals
i lo
# backtrace
bt
# quit
q
```
