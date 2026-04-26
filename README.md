# coreutils-static

Because we all need the most static coreutils we can get in this world.

Forked from: https://github.com/luciusmagn/coreutils-static 

## Pre-requisite
Install upx utility:

Ubuntu: `sudo apt-get install upx`

## Getting

Run `./build_on_mac.sh`. to build on Mac/Darwin

Run `./build_on_wsl.sh`. to build on Windows + WSL

Note that you really can't have truly static binaries on Darwin or
Windows machines, because there are no static libraries that can be used.

On Linux, we use musl instead of glibc to avoid `dlopen()`.
## What's the point of this?
I can run coreutils anywhere

## Screenshots
https://drive.google.com/file/d/1ugbBL1VF4pwyCNH0W-jsBYcw-LGhe63o/view?usp=sharing
