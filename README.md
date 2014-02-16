Compile a simple Linux distribution from souce code
Nanolinux is just for fun
E-mail: swn1012@126.com


1. Install compiler
   mkdir -p /opt
   mv nano_compiler.tar.bz2 /opt/
   cd /opt
   tar -jxf nano_compiler.tar.bz2
   
   
2. Build nanolinux image form source code
   1) Decompress
      tar -jxf nanolinux.tar.bz2
   2) Downlaod software
      Download the following packages to the directory "nanolinux/package":
      syslinux-6.02
      linux-3.10.20
      nasm-2.10.09
      gnu-efi-3.0
      busybox-1.22.1
      udev-182
      pkg-config-0.28
      util-linux-2.24
      ncurses-5.9
      glib-2.38.0
      libffi-3.0.13
      kmod-14
      usbutils-0.90
      libusb-0.1.12
      grub-2.00
      e2fsprogs-1.42.1
      Note:  gz bz2 xz file all OK.
   3) Compile
      cd nanolinux
      make
      Note: image path is nanolinux/platforms/x86/image/nanolinux.iso