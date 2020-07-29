## Kernel hacking links ((WIP))
A mess of links that have been helpful to me, adding them as I find them.  Hopefully this will save some people a lot of time on Google :) 
I'll try to organize them by topic as best as I can, and eventually add a table of contents.
These links assume that you're already comfortable in a *NIX environment and know your way around as a GNU/Linux user, i.e. shell commands & compiling your own kernels.

#### Books
- My 2 holy grails:
  - https://lwn.net/Kernel/LDD3/
  - https://www.amazon.com/Linux-Kernel-Development-Robert-Love/dp/0672329468
 - 
 
#### Getting started: first patches, coding style, & LKML etiquette
- https://kernelnewbies.org/
  - A plethora of resources, taking the time to check out what they have to offer is worth it. 
- https://www.kernel.org/doc/html/latest/process/submitting-patches.html
- https://www.kernel.org/doc/html/latest/process/email-clients.html
- https://www.kernel.org/doc/html/latest/process/coding-style.html
- http://tuxdiary.com/2015/03/22/check-kernel-code-checkpatch/
- https://www.kernel.org/doc/html/latest/kbuild/index.html
  - All about compiling kernels, from kconfig to Makefiles, GCC to Clang.
- https://lore.kernel.org/lkml/
- https://kernelnewbies.org/OutreachyRebase
- https://www.kernel.org/doc/html/latest/maintainer/rebasing-and-merging.html
- https://git-scm.com/book/en/v2/Git-Branching-Rebasing

#### Work environment
- http://cscope.sourceforge.net/cscope_vim_tutorial.html
- https://medium.com/code-dementia/how-cscope-makes-my-life-easier-6a0f13ca79e6

#### Kernels
- linux-next
  - https://www.kernel.org/doc/man-pages/linux-next.html
  - https://www.man7.org/linux/man-pages/man8/debugfs.8.html
  - https://www.kernel.org/doc/html/latest/filesystems/debugfs.html

#### Debugging
- https://static.lwn.net/images/pdf/LDD3/ch04.pdf
- https://d3s.mff.cuni.cz/files/teaching/nswi161/slides/06_debugging.pdf
- Oops & panics
  - http://www.gonehiking.org/ShuahLinuxBlogs/blog/2018/10/21/the-linux-kernel-has-bugs-really/
  - https://sanjeev1sharma.wordpress.com/tag/debug-kernel-panics/
  - https://www.opensourceforu.com/2011/01/understanding-a-kernel-oops/
  - http://neependra.net/kernel/Debugging_Kernel_OOPs_FUDCon2011.pdf
  - https://www.kernel.org/doc/html/latest/admin-guide/bug-hunting.html
  - https://lwn.net/Articles/592724/ (decode_stacktrace)
  - https://blog.seibert-media.com/2018/01/04/log-book-linux-cpu-lockups/
  - http://www.inetservicescloud.com/knowledgebase/what-is-a-cpu-soft-lockup/
 - Tools
  - https://www.kernel.org/doc/html/latest/dev-tools/gdb-kernel-debugging.html
  - https://linux.die.net/man/1/objdump
 - KASAN
  - https://www.kernel.org/doc/html/latest/dev-tools/kasan.html?highlight=kasan
  - https://lwn.net/Articles/618180/
  - https://events.static.linuxfound.org/sites/events/files/slides/LinuxCon%20North%20America%202015%20KernelAddressSanitizer.pdf
  - https://patchwork.kernel.org/cover/10579913/
  - https://blog.fuzzing-project.org/23-Kernel-Address-Sanitizer-KASAN.html
  - https://cwe.mitre.org/data/definitions/416.html
  - https://securityintelligence.com/use-after-frees-that-pointer-may-be-pointing-to-something-bad/

#### Module basics
- https://static.lwn.net/images/pdf/LDD3/ch13.pdf
- https://static.lwn.net/images/pdf/LDD3/ch14.pdf
- https://www.kernel.org/doc/html/v4.13/driver-api/usb/writing_usb_driver.html
- https://www.kernel.org/doc/html/v4.13/driver-api/usb/usb.html
- https://www.kernel.org/doc/html/v4.13/driver-api/usb/hotplug.html
- https://elixir.bootlin.com/linux/v2.6.33/source/include/linux/hid.h#L34
- https://elixir.bootlin.com/linux/latest/source/include/linux/printk.h
- https://elixir.bootlin.com/linux/latest/source/include/linux/init.h
- https://elixir.bootlin.com/linux/latest/source/include/linux/kernel.h

#### Misc device drivers
- https://linux-kernel-labs.github.io/refs/heads/master/labs/device_drivers.html#read-and-write
- https://www.kernel.org/doc/html/latest/driver-api/misc_devices.html#c.misc_register
- https://embetronicx.com/tutorials/linux/device-drivers/misc-device-driver/
- https://embetronicx.com/tutorials/linux/device-drivers/cdev-structure-and-file-operations-of-character-drivers/
- https://static.lwn.net/images/pdf/LDD3/ch03.pdf
- https://www.kernel.org/doc/htmldocs/kernel-hacking/routines-copy.html
- https://www.fsl.cs.sunysb.edu/kernel-api/re257.html
- https://elixir.bootlin.com/linux/latest/source/include/linux/uaccess.h

#### debugfs
- https://www.kernel.org/doc/html/latest/filesystems/debugfs.html#id2
- https://www.kernel.org/doc/html/latest/locking/mutex-design.html#when-to-use-mutexes
- https://www.kernel.org/doc/html/v4.13/kernel-hacking/locking.html#mutex-api-reference
- https://www.zachpfeffer.com/single-post/A-Quick-debugfs-Example
- https://cyberglory.wordpress.com/2011/08/21/jiffies-in-linux-kernel/

#### sysfs
- https://www.kernel.org/doc/html/latest/admin-guide/sysfs-rules.html
- https://www.kernel.org/doc/html/latest/filesystems/sysfs.html
- https://www.kernel.org/doc/html/latest/core-api/kernel-api.html#c.snprintf
- https://www.kernel.org/doc/html/latest/hwmon/sysfs-interface.html
- https://elixir.bootlin.com/linux/v4.14.5/source/Documentation/kobject.txt
- books.gigatux.nl/mirror/kerneldevelopment/0672327201/ch17lev1sec8.html
- https://elixir.bootlin.com/linux/latest/source/lib/vsprintf.c
- https://www.kernel.org/doc/htmldocs/kernel-api/API-snprintf.html

#### Linked lists
- https://www.fsl.cs.sunysb.edu/kernel-api/re252.html
- https://www.kernel.org/doc/htmldocs/kernel-api/API-strncpy.html
- http://books.gigatux.nl/mirror/kerneldevelopment/0672327201/ch11lev1sec4.html
- https://elixir.bootlin.com/linux/latest/source/include/linux/list.h
- https://linux.die.net/man/3/strncpy

#### Memory management
- https://www.tldp.org/LDP/tlk/mm/memory.html
- https://www.kernel.org/doc/html/latest/admin-guide/mm/concepts.html
- https://www.win.tue.nl/~aeb/linux/lk/lk-9.html
- https://en.wikibooks.org/wiki/The_Linux_Kernel/Memory
- https://www.youtube.com/watch?v=7aONIVSXiJ8
- https://static.lwn.net/images/pdf/LDD3/ch15.pdf
- https://learnlinuxconcepts.blogspot.com/2014/03/memory-layout-of-userspace-c-program.html
- https://developer.ibm.com/articles/l-kernel-memory-access/
- https://www.kernel.org/doc/html/v5.3/x86/exception-tables.html
- https://www.halolinux.us/kernel-reference/handling-the-tlb.html

#### TTY
- https://www.kernel.org/doc/html/latest/driver-api/serial/tty.html
- https://static.lwn.net/images/pdf/LDD3/ch18.pdf
- https://www.win.tue.nl/~aeb/linux/lk/lk-11.html

#### ASM/compiler stuff/etc
- https://refspecs.linuxbase.org/elf/gabi4+/ch4.reloc.html
- https://stffrdhrn.github.io/hardware/embedded/openrisc/2019/11/29/relocs.html
- https://docs.oracle.com/cd/E19641-01/802-1948/802-1948.pdf
- https://en.wikipedia.org/wiki/X86_instruction_listings
- https://refspecs.linuxbase.org/elf/x86_64-abi-0.98.pdf

#### Fuzzing/testing
- https://www.collabora.com/news-and-blog/blog/2020/04/17/using-syzkaller-to-detect-programming-bugs-in-linux/
- https://github.com/google/syzkaller/blob/master/docs/linux/setup.md
- https://github.com/google/syzkaller/blob/master/docs/linux/setup_ubuntu-host_qemu-vm_x86-64-kernel.md
- https://github.com/google/syzkaller/blob/master/docs/linux/kernel_configs.md
- https://github.com/dvyukov/syzkaller-repros
- https://groups.google.com/g/syzkaller/c/QbWWce5bPHc/m/zhSeTweOCAAJ
- https://groups.google.com/d/msg/syzkaller/RNp5Bg5pQZY/GwJ0KRqwBwAJ
- https://groups.google.com/d/msg/syzkaller/RQFLqAvdsEc/SHhXv50qCwAJ
- https://git.kernel.org/pub/scm/linux/kernel/git/shuah/linux-arts.git/
- https://github.com/google/syzkaller/blob/master/docs/reproducing_crashes.md
- https://github.com/google/syzkaller/blob/master/docs/executing_syzkaller_programs.md
