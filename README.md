C-INTERCAL can be a bit difficult to compile and install. Here's a combination of source code updates by Ais523 (to make it work on modern compilers) only accessible from a nethack4.org github link and the configure script (necessary to do the entire process) only accessible from Eric S. Raymond's site.

# Directions for Linux or WSL
- Extract c-intercal.tar.gz using the shell command `tar -xzvf c-intercal.tar.gz`. There should now be a folder called `c-intercal` in your current directory.
  - It's very important you use this shell tool and not Windows archiving tools like 7-zip. There are some important permissions on the files that only Unix tools will retain.
- Change to the new directory using `cd c-intercal`.
- For these next steps, you need the packages `build-essential`, `bison`, and `flex`. These are easy to get with the apt package manager on Ubuntu/Debian. Sometimes the `build-essential` package can be a bit tricky; you could try installing the packages separately (`gcc`, `g++`, `libc6-dev`, `make`, `dpkg-dev`) or consult [this thread](https://askubuntu.com/questions/398489/how-to-install-build-essential) for some possible solutions.
- Run `./configure` in the shell
- Run `make` in the shell.
- Run `make install` in the shell.
- C-INTERCAL should now be installed on your system. Call it from anywhere with `ick`.
