# asterisk-aac
Advanced Audio Coding format module for asterisk

## Prereq

### Debian based OS-es

sudo apt install libfaac-dev libfaad-dev

### RedHat based OS-es

#### Repository

1. Add the https://rpmfusion.org/ repository to your system.
1. Enable the non-free respotiory

## Install

### Patch asterisk sources

Apply the provided `format_aac.patch` on the Asterisk source tree.

### Copy module source

Copy the provided `formats/format_aac.c` to the formats/ directory of the Asterisk source tree.

## Reconfigure

1. Install autoconf: sudo ./contrib/script/install_prereq.sh install
1. Regenerate the configure script ./bootstrap.sh
1. Reconfigure asterisk: ./configure

## Enable the module & compile Asterisk

1. make menuconfig
1. make install