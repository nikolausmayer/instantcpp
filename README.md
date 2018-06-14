
instantcpp
==========

Execute C++ code snippets, directly on the command line.

```
$ instantcpp 'std::cout << "Hello World!" << std::cout;'
Hello World!
```

<b>instantcpp</b> gently grabs your naked C++ snippet, lovingly wraps it in a tiny warm blanket of cozy boilerplate code, compiles and executes the whole burrito, and then it even cleans up after itself. How nice!


Usage
=====

`instantcpp [options] <code>`

Options
-------
* `--cxx=<value>`, `--cxx <value>`: Use a custom compiler (instead of `g++`)
* `--valgrind`: Execute snipped in Valgrind
* `--gdb`: Execute snipped in GDB
* `-c <value>`: Add an option to compiler flags. Default is `-W -Wall -Wextra -Wpedantic -std=c++11 -O0` (fairly many warnings, C++11, no optimization).
* `-l <value>`: Add an option to linker flags. None by default.
* `-i <value>`: Add another `#include` to the wrapper code. See [code](instantcpp#194) for defaults.


