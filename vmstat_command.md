## ```vmstat``` command
- install command : sudo apt-get install sysstat
- shows version : vmstat -V
- show help page : vmstat -h or vmstat --help
- to display system information in six sections : vmstat
- to display active and inactive system memory : vmstat -a
- to memory and scheduling statistics : vmstat -s
- to display number of forks since boot : vmstat -f
- to display quick summary statistic of all disk activity : vmstat -D
- to get a detailed statistic on each disk usage : vmstat -d
- to generate a report related to a specific partition : vmstat -p sda1 (vmstat -p partition_identifier)
- to display timestamp information for updates : vmstat -t
- to display time elapsed between each output update : vmstat 5 (vmstat delay)
- to display how many updates to carry out before the output stops refreshing : vmstat 3 3 (vmstat delay count)
- to change the output units : vmstat 3 3 -S M (vmstat -S k/K/m/M)
- to display statistics for slabs : sudo vmstat -m






### Six section
- procs – Process Statistics
    - r – Active process count.
    - b – Sleeping process count.
- memory – Memory statistics
    - swpd – Total virtual memory. The swap space is initially unoccupied. However, the kernel starts using swap space as the system’s physical memory reaches its limit.
    - free – Total free memory.
    - buff – Total memory temporarily used as a data buffer.
    - cache – Total cache memory.
- swap – Swap space Statistics
    - si – The rate of swapping-in memory from disk.
    - so – The rate of swapping-out memory to disk.
- io – Input/Output Statistics
    - bi – Blocks received from a block device per second.
    - bo – Blocks sent to a block device per second.
- system – Scheduling statistics
    - in – The number of system interrupts.
    - cs – The number of context switches per second.
- cpu – CPU Statistics
    - us – The percentage of CPU time spent on non-kernel processes.
    - sy – The percentage of CPU time spent on kernel processes.
    - id – The percentage of idle CPU.
    - wa – The percentage of CPU time spent waiting for Input/Output.
    - st – The percentage of CPU time stolen by a virtual machine.



