#Linux works on ASK architecture

    A:Application
    
    S:Shell
    
    K:Kernel

To interact with hardware there is an application used eg; Terminal.

    Application- just like terminal used to execute any process via command eg; cd->change directory, mkdir-> make directory, rm->remove ,cp->copy ,mv->move or remane.
    
    Shell- An interface between the user and the kernel. It interprets commands and executes them.
    
    Kernal-The core component of Linux, acting as a bridge between hardware and software.

--------------------------------------------------------------------------------------------------------

Systemd is a system and service manager for modern Linux operating systems. It initializes the system, manages services, and controls system resources during startup and runtime. Systemd replaces the traditional SysV init system and runs as the first process with Process ID (PID) 1.

    1.Initialize the system during boot
    2.Manage and control system services
    3.Replace the traditional SysV init system
    4.Improve boot speed and performance
    5.Provide centralized system management tools

Useful process commands--

view process:

    ps aux
    top
    htop

Kill process:

    kill PID
    kill -9 PID


--------------------------------------------------------------------------------------------------------------

Process States:

1. Running (R)-Process is currently using CPU or ready to run.

Command used to see all R state processes:

    top

2. Sleeping (S) Interruptible Sleep -Process is waiting for something (like I/O).

        Process is waiting for something (like I/O).
        Can be woken up easily.

Example:

    Waiting for user input.
    Waiting for file read.

3. Uninterruptible Sleep -

        Waiting for critical I/O (like disk)
        Cannot be interrupted easily

Important:

    Even kill -9 may not work immediately

4. Stopped (T)

        Process is paused/stopped.
        Usually by user(ctrl+c).

5. Zombie (Z)-Process is dead but still in process table.

To see all such process:

    ps aux | grep Z


  ------------------------------------------------------------------------------------------
  "In Linux, a process can be in different states such as Running, Sleeping, Uninterruptible Sleep, Stopped, and Zombie. These states represent whether a process is executing, waiting for resources, paused, or finished but not cleaned up. These states help the operating system efficiently manage CPU and resources."
























