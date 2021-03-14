# HOW LINUX WORKS

[Book Description](https://www.oreilly.com/library/view/how-linux-works/9781457185519/)

# HOW LINUX WORKS

[Linux Road Map](linux_Roadmap.md)

## Chapter 01 - The Big Picture

- Level and Layers of Abstraction in a Linux System
  - Hardware
  - Linux Kernel
  - User process
- Hardware: Understanding Main Memory
    > Of all the hardware on a computer system, *main memory* is perhaps the most important.
- The Kernel is in charge of managing task in four several system areas:
  - Process
  - Memory
  - Device drives
  - System calls and support
- Process Management
    > *Process management* describe hte starting, pausing, resuming, and terminating of processes.
- Memory Management
- Device Drives and Management
- System Call and Support
- User Space
- Users
  - root
- Look Forward
    > So far, you've seen what makes up a *running* Linux system. User processes make up the environment that you directly interact whit; the kernel manages processes and hardware. Both the kernel and processes reside in memory.
    This is great background information, but you can't learn the details of a Linus system by reading about it alone; you need to get yours hands dirty. The next chapter stars your journey b teaching you some user-spaces basics. Along the way, you'll learn about a major part of the Linux system that this chapter doesn't discuss - long-term storages (disk, files, etc.). After all, you need to store you programs and data somewhere.

## Chapter 02 - Basic Commands and Directory Hierarchy

- Using the Shell
  - cat
  - echo
  - 

- The Bourne Shell: **/bin/sh**

```bash
    $echo Hello there.
    cat /etc/passwd
```

<https://www.youtube.com/playlist?list=PLacuG5pysFbDQU8kKxbUh4K5c1iL5_k7k>

<https://www.youtube.com/playlist?list=PLhwVAYxlh5dsX6aOfVMZXS8MwKwBmwVM6>

## Basic Commands

```bash
ls
cp
mv
touch
rm
echo
cd
mkdir
rmdir
rm -rf
echo *
```

## Intermediate Commands

```bash
grep
less
pwd
diff
file
find
head
teal
sort
STUFF=blah
export STUFF
echo $STUFF
$PATH
```
Keystroke | Action
---|---
**CTRL + B** | Move hte cursor for left


## Chapter 01 - The Big Picture

So far, you've seen what makes up a *running* Linux system. User processes make up the environment that you directly interact with; the kernel manages processes and hardware. Both the kernel and precesses reside in memory.

This is great background information, but you can't learn the details of a Linux system by reading about it alone; you need to get your hands dirty. The next chapter starts your journey by teaching you some user-space basics. ALong the way, you'll learn about a major part of the Linux system that this chapter doesn't discuss -- long-term storage (disks, files, etc.). After all, you need to stores your programs and data somewhere.

## Chapter 02 - Basic Commands and Directory Hierarchy
