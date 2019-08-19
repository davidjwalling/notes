# Using GDB
### GDB Initialization File for Fedora 30
##### Confirm GDB Version
```
$ gdb --version
GNU gdb (GDB) Fedora 8.3-6.fc30
Copyright (C) 2019 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.
$
```
##### Setup the GDB User Defaults File (~/.gdbinit)
If curses window management is availble
```
$ vi ~/.gdbinit
set breakpoint pending on
set pagination off
enable tui
layout regs
winheight regs 6
winheight src 30
define hook-next
  refresh
end
define hook-quit
  set confirm off
end
:x
$
```
If curses window management is not availble
```
$ vi ~/.gdbinit
set breakpoint pending on
set pagination off
set tui border-kind ascii
layout regs
winheight regs 6
winheight src 30
define hook-next
  refresh
end
define hook-quit
  set confirm off
end
:x
$
```
### Create a GDB Project Command File
```
$ cd ~/myproject
# vi myproject.gdb
file myproject
break main
run
:x
$
```
