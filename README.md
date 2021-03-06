# Learning GoogleTest

Working through the official getting started material and guides in the [GoogleTest User's Guide](https://google.github.io/googletest/). GoogleTest is a unit testing framework for the C++ programming language. Intention is to get a better understanding on how to work with GoogleTest and also unit testing in general.

## My Platform

Will use different platform combinations but a common setup can be the below listed.

### Operating System

Mostly running Windows both at work and at home. The PC that this paragraph is written on is currently running Windows 10 Pro, version 21H1.

### Compilers

Have multiple C++ compilers:

- GCC 8.1.0 (x86_64-posix-seh-rev0, Built by MinGW-W64 project)
- Clang 13.0.0 (through the LLVM project)
- MSVC 19.29 (through Visual Studio community edition)

### Build Systems

Have multiple build systems:

- Cmake 3.23.0
- Bazel 4.2.1

## Quick Start CMake

Made a project in the folder `google-test-quick-start-cmake`. This project consists of a C++ file with tests and a file with instructions for CMake.

Built and ran the tests in the project from the command line when in the project folder using the commands:

```txt
cmake -S . -B build
```

```txt
cmake --build build
```

```txt
cd build
```

```txt
ctest
```

The output from the last `ctest` command was:

```txt
 Start 1: HelloTest.BasicAssertions
1/1 Test #1: HelloTest.BasicAssertions ........   Passed    0.21 sec

100% tests passed, 0 tests failed out of 1

Total Test time (real) =   0.29 sec
```

From the output it can be seen that one test ran and this test passed.
