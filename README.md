# build-a-pi
# set build environment
- host:
 > x86-64  
 > wsl2  
 > yan@YAN:~/build_mypi/qemu-2.11.0$ lsb_release -a  
 > LSB Version:    core-11.1.0ubuntu2-noarch:security-11.1.0ubuntu2-noarch  
 > Distributor ID: Ubuntu  
 > Description:    Ubuntu 20.04.2 LTS  
 > Release:        20.04  
 > Codename:       focal  
- select your compiler-> gcc-arm-11.2-2022.02-x86_64-arm-none-eabi.tar.xz  
  - https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/downloads
- install qemu
  - wget https://download.qemu.org/qemu-2.11.0.tar.xz
  - tar xvf ./qemu-2.11.0.tar.xz
  - cd qemu-2.11.0
  - some patchs
    - https://blog.csdn.net/newnewman80/article/details/90175033
    - https://gitlab.com/qemu-project/qemu/-/issues/135
    - https://patchwork.kernel.org/project/qemu-devel/patch/20190617114005.24603-1-berrange@redhat.com/#22706395
    - https://isrc.iscas.ac.cn/gitlab/mirrors/github.com/openembedded_openembedded-core/-/commit/1351f9be973cfbd043f9b10d218e3cecaa0ab372

# miscellaneous stuff
- https://stackoverflow.com/questions/5961701/arm-gcc-toolchain-as-arm-elf-or-arm-none-eabi-what-is-the-difference
