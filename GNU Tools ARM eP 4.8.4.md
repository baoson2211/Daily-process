# GNU Tools for ARM Embedded Processors
# Version: 4.8

## Table of Contents
1. Installing executables on Linux
2. Installing executables on Mac OS X
3. Installing executables on Windows 
4. Invoking GCC
5. Architecture options usage
6. C Libraries usage
7. GCC Plugin usage
8. Linker scripts & startup code
9. Samples
10. GDB Server for CMSIS-DAP based hardware debugger

## 1. Installing executables on Linux 
Unpack the tarball to the install directory, like this:<br />
```$ cd $install_dir && tar xjf gcc-arm-none-eabi-*-yyyymmdd-linux.tar.bz2```

For 64 bit system, 32 bit libc and libncurses are required to run the tools.

For some Ubuntu releases, the toolchain can also be installed via
Launchpad PPA at [https://launchpad.net/~terry.guo/+archive/gcc-arm-embedded](https://launchpad.net/~terry.guo/+archive/gcc-arm-embedded).

## 2. Installing executables on Mac OS X
Unpack the tarball to the install directory, like this:<br />
```$ cd $install_dir && tar xjf gcc-arm-none-eabi-*-yyyymmdd-mac.tar.bz2```

## 3. Installing executables on Windows
Run the installer ```(gcc-arm-none-eabi-*-yyyymmdd-win32.exe)``` and follow the
instructions.

The toolchain in windows ```zip``` package is a backup to windows installer for
those who cannot run installer.  We need decompress the zip package
in a proper place and then invoke it following instructions in next section.

## 4. Invoking GCC 
On Linux and Mac OS X, either invoke with the complete path like this:<br />
```$ $install_dir/gcc-arm-none-eabi-*/bin/arm-none-eabi-gcc```

Or set path like this:<br />
```$ export PATH=$PATH:$install_dir/gcc-arm-none-eabi-*/bin```
```$ arm-none-eabi-gcc```

On Windows (although the above approaches also work), it can be more
convenient to either have the installer register environment variables, or run
```INSTALL_DIR\bin\gccvar.bat``` to set environment variables for the current cmd.

For windows ```zip``` package, after decompression we can invoke toolchain either with
complete path like this:<br />
```TOOLCHAIN_UNZIP_DIR\bin\arm-none-eabi-gcc```<br />
or run ```TOOLCHAIN_UNZIP_DIR\bin\gccvar.bat``` to set environment variables for the
current cmd.

## 5. Architecture options usage

This toolchain is built and optimized for Cortex-A/R/M bare metal development.
the following table shows how to invoke GCC/G++ with correct command line
options for variants of Cortex-A/R and Cortex-M architectures. <br />
```
--------------------------------------------------------------------
| ARM Core | Command Line Options                       | multilib |
|----------|--------------------------------------------|----------|
|Cortex-M0+| -mthumb -mcpu=cortex-m0plus                | armv6-m  |
|Cortex-M0 | -mthumb -mcpu=cortex-m0                    |          |
|Cortex-M1 | -mthumb -mcpu=cortex-m1                    |          |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv6-m                     |          |
|----------|--------------------------------------------|----------|
|Cortex-M3 | -mthumb -mcpu=cortex-m3                    | armv7-m  |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7-m                     |          |
|----------|--------------------------------------------|----------|
|Cortex-M4 | -mthumb -mcpu=cortex-m4                    | armv7e-m |
|(No FP)   |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m                    |          |
|----------|--------------------------------------------|----------|
|Cortex-M4 | -mthumb -mcpu=cortex-m4 -mfloat-abi=softfp | armv7e-m |
|(Soft FP) | -mfpu=fpv4-sp-d16                          | /softfp  |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m -mfloat-abi=softfp |          |
|          | -mfpu=fpv4-sp-d16                          |          |
|----------|--------------------------------------------|----------|
|Cortex-M4 | -mthumb -mcpu=cortex-m4 -mfloat-abi=hard   | armv7e-m |
|(Hard FP) | -mfpu=fpv4-sp-d16                          | /fpu     |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m -mfloat-abi=hard   |          |
|          | -mfpu=fpv4-sp-d16                          |          |
|----------|--------------------------------------------|----------|
|Cortex-M7 | -mthumb -mcpu=cortex-m7                    | armv7e-m |
|(No FP)   |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m                    |          |
|----------|--------------------------------------------|----------|
|Cortex-M7 | -mthumb -mcpu=cortex-m7 -mfloat-abi=softfp | armv7e-m |
|(Soft FP) | -mfpu=fpv5-sp-d16                          | /softfp  |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m -mfloat-abi=softfp |          |
|          | -mfpu=fpv5-sp-d16                          |          |
|          |--------------------------------------------|          |
|          | -mthumb -mcpu=cortex-m7 -mfloat-abi=softfp |          |
|          | -mfpu=fpv5-d16                             |          |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m -mfloat-abi=softfp |          |
|          | -mfpu=fpv5-d16                             |          |
|----------|--------------------------------------------|----------|
|Cortex-M7 | -mthumb -mcpu=cortex-m7 -mfloat-abi=hard   | armv7e-m |
|(Hard FP) | -mfpu=fpv5-sp-d16                          | /fpu     |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m -mfloat-abi=hard   |          |
|          | -mfpu=fpv5-sp-d16                          |          |
|          |--------------------------------------------|          |
|          | -mthumb -mcpu=cortex-m7 -mfloat-abi=hard   |          |
|          | -mfpu=fpv5-d16                             |          |
|          |--------------------------------------------|          |
|          | -mthumb -march=armv7e-m -mfloat-abi=hard   |          |
|          | -mfpu=fpv5-d16                             |          |
|----------|--------------------------------------------|----------|
|Cortex-R4 | [-mthumb] -march=armv7-r                   | armv7-ar |
|Cortex-R5 |                                            | /thumb   |
|Cortex-R7 |                                            |          |
|(No FP)   |                                            |          |
|----------|--------------------------------------------|----------|
|Cortex-R4 | [-mthumb] -march=armv7-r -mfloat-abi=softfp| armv7-ar |
|Cortex-R5 | -mfpu=vfpv3-d16                            | /thumb   |
|Cortex-R7 |                                            | /softfp  |
|(Soft FP) |                                            |          |
|----------|--------------------------------------------|----------|
|Cortex-R4 | [-mthumb] -march=armv7-r -mfloat-abi=hard  | armv7-ar |
|Cortex-R5 | -mfpu=vfpv3-d16                            | /thumb   |
|Cortex-R7 |                                            | /fpu     |
|(Hard FP) |                                            |          |
|----------|--------------------------------------------|----------|
|Cortex-A* | [-mthumb] -march=armv7-a                   | armv7-ar |
|(No FP)   |                                            | /thumb   |
|----------|--------------------------------------------|----------|
|Cortex-A* | [-mthumb] -march=armv7-a -mfloat-abi=softfp| armv7-ar |
|(Soft FP) | -mfpu=vfpv3-d16                            | /thumb   |
|          |                                            | /softfp  |
|----------|--------------------------------------------|----------|
|Cortex-A* | [-mthumb] -march=armv7-a -mfloat-abi=hard  | armv7-ar |
|(Hard FP) | -mfpu=vfpv3-d16                            | /thumb   |
|          |                                            | /fpu     |
--------------------------------------------------------------------
```

## 6. C Libraries usage

This toolchain is released with two prebuilt C libraries based on newlib:
one is the standard newlib and the other is newlib-nano for code size.
To distinguish them, we rename the size optimized libraries as:

  ```libc.a --> libc_s.a```<br />
  ```libg.a --> libg_s.a```

To use newlib-nano, users should provide additional gcc link time option:<br />
 ```--specs=nano.specs```<br />

Nano.specs also handles two additional gcc libraries: ```libstdc++_s.a``` and
```libsupc++_s.a```, which are optimized for code size.<br />

For example:<br />
```$ arm-none-eabi-gcc src.c --specs=nano.specs $(OTHER_OPTIONS)```<br />

This option can also work together with other specs options like
```--specs=rdimon.specs```<br />

Please be noticed that ```--specs=nano.specs``` is a linker option. Be sure
to include in linker option if compiling and linking are separated.

##### 6.1. additional newlib-nano libraries usage

Newlib-nano is different from newlib in addition to the libraries' name.
Formatted input/output of floating-point number are implemented as weak symbol.
If you want to use %f, you have to pull in the symbol by explicitly specifying
```-u``` command option.
   
  ```-u _scanf_float```<br />
  ```-u _printf_float```

e.g. to output a float, the command line is like: <br />
```$ arm-none-eabi-gcc --specs=nano.specs -u _printf_float $(OTHER_LINK_OPTIONS)```

For more about the difference and usage, please refer the ```README.nano``` in the
source package.

Users can choose to use or not use semihosting by following instructions.

##### 6.2. semihosting
If you need semihosting, linking like:<br />
```$ arm-none-eabi-gcc --specs=rdimon.specs $(OTHER_LINK_OPTIONS)```

##### 6.3. non-semihosting/retarget
If you are using retarget, linking like:<br />
```$ arm-none-eabi-gcc --specs=nosys.specs $(OTHER_LINK_OPTIONS)```

## 7. GCC Plugin usage
This release includes following Linux GCC plugins for additional performance
optimization:

##### 7.1. tree_switch_shortcut: optimize (Finite State Machine) FSM style program
to reduce condition jump or indirect jumps. Usage:<br />
```(GCC option) -fplugin=tree_switch_shortcut_elf```

Please be noticed that current GCC plugin can only run on Linux host. They
are not available to Windows or Mac OS hosted GCC.

## 8. Linker scripts & startup code

Latest update of linker scripts template and startup code is available on 
[http://www.arm.com/cmsis](http://www.arm.com/cmsis).

## 9. Samples 
Examples of all above usages are available at:<br />
	```$install_dir/gcc-arm-none-eabi-*/share/gcc-arm-none-eabi/samples```

Read ```readme.txt```	 under it for further information.

## 10. GDB Server for CMSIS-DAP based hardware debugger
CMSIS-DAP is the interface firmware for a Debug Unit that connects
the Debug Port to USB.  More detailed information can be found at
[http://www.keil.com/support/man/docs/dapdebug/](http://www.keil.com/support/man/docs/dapdebug/).

A software GDB server is required for GDB to communicate with CMSIS-DAP based
hardware debugger.  The pyOCD is an implementation of such GDB server that is
written in Python and under Apache License.

For those who are using this toolchain and have board with CMSIS-DAP based
debugger, the pyOCD is our recommended gdb server.
More information can be found at [https://github.com/mbedmicro/pyOCD](https://github.com/mbedmicro/pyOCD).

Currently pyOCD is still in development stage but has a quite active community.
Reporting issues in either our Launchpad website or pyOCD community are welcomed.
