# UW-CSE451-Operating-System-Lab
This is a lab for UW cse 451 Operating System.

All of labs are based on the Experimental Kernel (i.e., xk). xk is a new experimental
operating system kernel for teaching the principles and practice of operating systems.
xk's baseline code is a complete, bootable operating system. It provides some simple system
calls that it is capable of running a “hello world” program. Your task in each lab is to make
xk complete and also add a few functionalities

All code are programmed in C

- Lab 1: Interrupts and System Calls
- Lab 2: Multiprocessing
- Lab 3: Address Space Management
- Lab 4: Filesystem

# Hướng dẫn thực hành
## B1: Tải những môi trường cần thiết.
- QEMU (Lưu ý: QEMU >= 2.9).
- sudo apt-get install libsdl2-dev
## B2: Build source
- Tải source code này về máy
- Tạo 1 thư mục tên là `xk`. Sau đó `copy` và `past` source code này vào trong thư mục đó.
- Gõ `make` vào ternimal.
=> Sau `B2` thì sẽ tạo ra thư mục `out`.

`NOTE`: Khi tải source code này về file `sign.pl` chưa được cấp quyền thực thi.
-> Để giải quyết: `chmod +x sign.pl`

## B3: Chạy xk-OS
- Gõ `make qemu` vào terminal.

Nếu thành công màn hình sẽ hiển thị:
~~~
SeaBIOS (version 1.13.0-1ubuntu1.1)


iPXE (http://ipxe.org) 00:03.0 CA00 PCI2.10 PnP PMM+00F8CA10+00ECCA10 CA00
                                                                               


Booting from Hard Disk..xk...
CPU: QEMU Virtual CPU version 2.5+
  fpu de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2
  sse3 cx16 hypervisor
  syscall nx lm
  lahf_lm svm
E820: physical memory map [mem 0x9000-0x908f]
  [mem 0x0-0x9fbff] available
  [mem 0x9fc00-0x9ffff] reserved
  [mem 0xf0000-0xfffff] reserved
  [mem 0x100000-0xfdffff] available
  [mem 0xfe0000-0xffffff] reserved
  [mem 0xfffc0000-0xffffffff] reserved

cpu0: starting xk

free pages: 3683
cpu0: starting
sb: size 100000 nblocks 34407 bmap start 65568 inodestart 65593
init: starting sh
$ QEMU: Terminated
~~~

- Để thoát khỏi qemu: Nhấn `Crtl + a` sau đó thả ra rồi nhấn phím `x` trên bàn phím.


  

