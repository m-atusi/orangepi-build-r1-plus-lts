for Orange Pi R1 Plus LTS on Wsl(jammy) environment

```
$ uname -a
Linux localvaio 5.15.79.1-microsoft-standard-WSL2 #1 SMP Wed Nov 23 01:01:46 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux
$ sudo ./build.sh
```


./output/images/Orangepir1plus-lts_2.2.2_ubuntu_focal_server_linux5.10.44_minimal/Orangepir1plus-lts_2.2.2_ubuntu_focal_server_linux5.10.44_minimal.img

<img width="731" alt="スクリーンショット 2023-02-24 134906" src="https://user-images.githubusercontent.com/59951021/221100023-44c8a493-4e29-4c61-a815-03446ceeb48c.png">

[Console]
```{r, max.height='100px'}

Orange Pi 2.2.2 Focal ttyS2 

orangepir1plus-lts login: 
orangepir1plus-lts login: 
orangepir1plus-lts login: DDR version 1.16 20190528
ID:0x805 N
In
LPDDR3
333MHz
Bus Width=32 Col=10 Bank=8 Row=14/14 CS=2 Die Bus-Width=32 Size=1024MB
ddrconfig:6
OUT
Boot1 Release Time: May 13 2019 17:34:36, version: 2.50
ChipType = 0x11, 240
mmc2:cmd1,20
emmc reinit
mmc2:cmd1,20
emmc reinit
mmc2:cmd1,20
SdmmcInit=2 1
mmc0:cmd5,20
SdmmcInit=0 0
BootCapSize=0
UserCapSize=30436MB
FwPartOffset=2000 , 0
StorageInit ok = 33637
Raw SecureMode = 0
SecureInit read PBA: 0x4
SecureInit read PBA: 0x404
SecureInit read PBA: 0x804
SecureInit read PBA: 0xc04
SecureInit read PBA: 0x1004
SecureInit ret = 0, SecureMode = 0
atags_set_bootdev: ret:(0)
GPT 0x337a9f0 signature is wrong
recovery gpt...
GPT 0x337a9f0 signature is wrong
recovery gpt fail!
LoadTrust Addr:0x4000
No find bl30.bin
No find bl32.bin
Load uboot, ReadLba = 2000
hdr 000000000337a3b0 + 0x0:0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,

Load OK, addr=0x200000, size=0xab6cc
RunBL31 0x40000
INFO:    Preloader serial: 2
NOTICE:  BL31: v1.3(debug):403e0b816
NOTICE:  BL31: Built : 14:13:08, Aug 11 2020
NOTICE:  BL31:Rockchip release version: v1.3
INFO:    ARM GICv2 driver initialized
INFO:    Using opteed sec cpu_context!
INFO:    boot cpu mask: 1
INFO:    plat_rockchip_pmu_init: pd status 0xe
INFO:    BL31: Initializing runtime services
WARNING: No OPTEE provided by BL2 boot loader, Booting device without OPTEE initialization. SMC`s destined for OPTEE will return SMC_UNK
ERROR:   Error initializing runtime service opteed_fast
INFO:    BL31: Preparing for EL3 exit to normal world
INFO:    Entry point address = 0x200000
INFO:    SPSR = 0x3c9


U-Boot 2020.10-orangepi (Feb 24 2023 - 07:41:50 +0900)

Model: Xunlong Orange Pi R1 Plus LTS
DRAM:  1022 MiB
PMIC:  RK8050 (on=0x10, off=0x00)
MMC:   mmc@ff500000: 1
Loading Environment from MMC... MMC Device 0 not found
*** Warning - No MMC card found, using default environment

In:    serial@ff130000
Out:   serial@ff130000
Err:   serial@ff130000
Model: Xunlong Orange Pi R1 Plus LTS
Net:   eth0: ethernet@ff540000
Hit any key to stop autoboot:  0 
switch to partitions #0, OK
mmc1 is current device
Scanning mmc 1:1...
Found U-Boot script /boot/boot.scr
3341 bytes read in 5 ms (652.3 KiB/s)
## Executing script at 00500000
Boot script loaded from mmc 1
230 bytes read in 3 ms (74.2 KiB/s)
14520118 bytes read in 633 ms (21.9 MiB/s)
28647936 bytes read in 1245 ms (21.9 MiB/s)
65295 bytes read in 9 ms (6.9 MiB/s)
2698 bytes read in 7 ms (376 KiB/s)
Applying kernel provided DT fixup script (rockchip-fixup.scr)
## Executing script at 09000000
Moving Image from 0x2080000 to 0x2200000, end=3df0000
## Loading init Ramdisk from Legacy Image at 06000000 ...
   Image Name:   uInitrd
   Image Type:   AArch64 Linux RAMDisk Image (gzip compressed)
   Data Size:    14520054 Bytes = 13.8 MiB
   Load Address: 00000000
   Entry Point:  00000000
   Verifying Checksum ... OK
## Flattened Device Tree blob at 01f00000
   Booting using the fdt blob at 0x1f00000
   Loading Ramdisk to 3d155000, end 3df2def6 ... OK
   Loading Device Tree to 000000003d0dc000, end 000000003d154fff ... OK

Starting kernel ...

Loading, please wait...
Starting version 245.4-4ubuntu3.19
Begin: Loading essential drivers ... done.
Begin: Running /scripts/init-premount ... done.
Begin: Mounting root file system ... Begin: Running /scripts/local-top ... done.
Begin: Running /scripts/local-premount ... done.
Begin: Will now check root file system ... fsck from util-linux 2.34
[/usr/sbin/fsck.ext4 (1) -- /dev/mmcblk0p1] fsck.ext4 -a -C0 /dev/mmcblk0p1 
/dev/mmcblk0p1: recovering journal
/dev/mmcblk0p1: clean, 22990/1865344 files, 354419/7706144 blocks
done.
done.
Begin: Running /scripts/local-bottom ... done.
Begin: Running /scripts/init-bottom ... done.

Welcome to Orange Pi 2.2.2 Focal!

[  OK  ] Created slice system-modprobe.slice.
[  OK  ] Created slice system-serial\x2dgetty.slice.
[  OK  ] Created slice User and Session Slice.
[  OK  ] Started Dispatch Password …ts to Console Directory Watch.
[  OK  ] Started Forward Password R…uests to Wall Directory Watch.
[  OK  ] Set up automount Arbitrary…s File System Automount Point.
[  OK  ] Reached target Local Encrypted Volumes.
[  OK  ] Reached target Remote File Systems.
[  OK  ] Reached target Slices.
[  OK  ] Reached target Swap.
[  OK  ] Reached target System Time Set.
[  OK  ] Listening on Syslog Socket.
[  OK  ] Listening on fsck to fsckd communication Socket.
[  OK  ] Listening on initctl Compatibility Named Pipe.
[  OK  ] Listening on Journal Audit Socket.
[  OK  ] Listening on Journal Socket (/dev/log).
[  OK  ] Listening on Journal Socket.
[  OK  ] Listening on udev Control Socket.
[  OK  ] Listening on udev Kernel Socket.
         Mounting Huge Pages File System...
         Mounting POSIX Message Queue File System...
         Mounting Kernel Debug File System...
         Mounting Kernel Trace File System...
         Starting Restore / save the current clock...
         Starting Set the console keyboard layout...
         Starting Create list of st…odes for the current kernel...
         Starting Load Kernel Module chromeos_pstore...
         Starting Load Kernel Module drm...
         Starting Load Kernel Module pstore_blk...
         Starting Load Kernel Module pstore_zone...
         Starting Load Kernel Module ramoops...
[  OK  ] Started Nameserver information manager.
[  OK  ] Reached target Network (Pre).
         Starting Load Kernel Modules...
         Starting Remount Root and Kernel File Systems...
         Starting udev Coldplug all Devices...
[  OK  ] Mounted Huge Pages File System.
[  OK  ] Mounted POSIX Message Queue File System.
[  OK  ] Mounted Kernel Debug File System.
[  OK  ] Mounted Kernel Trace File System.
[  OK  ] Finished Restore / save the current clock.
[  OK  ] Finished Create list of st… nodes for the current kernel.
[  OK  ] Finished Load Kernel Module chromeos_pstore.
[  OK  ] Finished Load Kernel Module drm.
[  OK  ] Finished Load Kernel Module pstore_blk.
[  OK  ] Finished Load Kernel Module pstore_zone.
[  OK  ] Finished Load Kernel Module ramoops.
[  OK  ] Finished Load Kernel Modules.
[  OK  ] Finished Remount Root and Kernel File Systems.
         Mounting FUSE Control File System...
         Mounting Kernel Configuration File System...
         Starting Load/Save Random Seed...
         Starting Apply Kernel Variables...
         Starting Create System Users...
[  OK  ] Mounted FUSE Control File System.
[  OK  ] Mounted Kernel Configuration File System.
[  OK  ] Finished Create System Users.
[  OK  ] Finished Apply Kernel Variables.
         Starting Create Static Device Nodes in /dev...
[  OK  ] Finished Set the console keyboard layout.
[  OK  ] Finished Create Static Device Nodes in /dev.
[  OK  ] Reached target Local File Systems (Pre).
         Mounting /tmp...
         Starting udev Kernel Device Manager...
[  OK  ] Mounted /tmp.
[  OK  ] Reached target Local File Systems.
         Starting Set console font and keymap...
         Starting Orange Pi ZRAM config...
[  OK  ] Finished Set console font and keymap.
[  OK  ] Started udev Kernel Device Manager.
[  OK  ] Finished udev Coldplug all Devices.
         Starting Helper to synchronize boot up for ifupdown...
[  OK  ] Found device /dev/ttyGS0.
[  OK  ] Finished Helper to synchronize boot up for ifupdown.
         Starting Raise network interfaces...
[  OK  ] Finished Raise network interfaces.
[  OK  ] Found device /dev/ttyS2.
[  OK  ] Finished Load/Save Random Seed.
[  OK  ] Finished Orange Pi ZRAM config.
         Starting Orange Pi memory supported logging...
[  OK  ] Finished Orange Pi memory supported logging.
         Starting Journal Service...
[  OK  ] Started Journal Service.
         Starting Flush Journal to Persistent Storage...
[  OK  ] Finished Flush Journal to Persistent Storage.
         Starting Create Volatile Files and Directories...
[  OK  ] Finished Create Volatile Files and Directories.
         Starting Network Name Resolution...
         Starting Update UTMP about System Boot/Shutdown...
[  OK  ] Finished Update UTMP about System Boot/Shutdown.
[  OK  ] Reached target System Initialization.
[  OK  ] Started resolvconf-pull-resolved.path.
[  OK  ] Started Daily Cleanup of Temporary Directories.
[  OK  ] Reached target Paths.
[  OK  ] Listening on D-Bus System Message Bus Socket.
[  OK  ] Reached target Sockets.
         Starting Orange Pi hardware monitoring...
         Starting Orange Pi hardware optimization...
[  OK  ] Finished Orange Pi hardware monitoring.
[  OK  ] Finished Orange Pi hardware optimization.
[  OK  ] Reached target Basic System.
[  OK  ] Started Regular background program processing daemon.
[  OK  ] Started D-Bus System Message Bus.
         Starting Network Manager...
[  OK  ] Started Save initial kernel messages after boot.
         Starting Remove Stale Onli…t4 Metadata Check Snapshots...
         Starting LSB: Load kernel …d to enable cpufreq scaling...
         Starting System Logging Service...
         Starting Resets System Activity Data Collector...
         Starting Login Service...
         Starting WPA supplicant...
[  OK  ] Finished Resets System Activity Data Collector.
[  OK  ] Started System Logging Service.
[  OK  ] Finished Remove Stale Onli…ext4 Metadata Check Snapshots.
[  OK  ] Started WPA supplicant.
[  OK  ] Started Network Name Resolution.
[  OK  ] Reached target Host and Network Name Lookups.
         Starting resolvconf-pull-resolved.service...
[  OK  ] Started Login Service.
[  OK  ] Started LSB: Load kernel m…ded to enable cpufreq scaling.
         Starting LSB: set CPUFreq kernel parameters...
[  OK  ] Started Network Manager.
[  OK  ] Finished resolvconf-pull-resolved.service.
[  OK  ] Started LSB: set CPUFreq kernel parameters.
[  OK  ] Reached target Network.
[  OK  ] Reached target Network is Online.
         Starting chrony, an NTP client/server...
         Starting /etc/rc.local Compatibility...
         Starting OpenBSD Secure Shell server...
         Starting LSB: Set sysfs variables from /etc/sysfs.conf...
         Starting Permit User Sessions...
         Starting Hostname Service...
[  OK  ] Started LSB: Set sysfs variables from /etc/sysfs.conf.
[  OK  ] Finished Permit User Sessions.
         Starting Set console scheme...
[  OK  ] Finished Set console scheme.
[  OK  ] Started chrony, an NTP client/server.
[  OK  ] Created slice system-getty.slice.
[  OK  ] Reached target System Time Synchronized.
[  OK  ] Started Daily apt download activities.
[  OK  ] Started Daily apt upgrade and clean activities.
[  OK  ] Started Periodic ext4 Onli…ata Check for All Filesystems.
[  OK  ] Started Discard unused blocks once a week.
[  OK  ] Started Daily rotation of log files.
[  OK  ] Started Message of the Day.
[  OK  ] Reached target Timers.
[  OK  ] Started /etc/rc.local Compatibility.
[  OK  ] Started Getty on tty1.
[  OK  ] Started Serial Getty on ttyGS0.
[  OK  ] Started Serial Getty on ttyS2.
[  OK  ] Reached target Login Prompts.
[  OK  ] Started OpenBSD Secure Shell server.
[  OK  ] Reached target Multi-User System.
[  OK  ] Reached target Graphical Interface.
         Starting Update UTMP about System Runlevel Changes...
[  OK  ] Finished Update UTMP about System Runlevel Changes.
[  OK  ] Started Hostname Service.

Orange Pi 2.2.2 Focal ttyS2 

orangepir1plus-lts login: 

```

[dmesg]
```{r, max.height='100px'}
[    0.000000] Booting Linux on physical CPU 0x0000000000 [0x410fd034]
[    0.000000] Linux version 5.10.44-rockchip64 (root@localvaio) (aarch64-none-linux-gnu-gcc (GNU Toolchain for the A-profile Architecture 9.2-2019.12 (arm-9.10)) 9.2.1 20191025, GNU ld (GNU Toolchain for the A-profile Architecture 9.2-2019.12 (arm-9.10)) 2.33.1.20191209) #2.2.2 SMP PREEMPT Fri Feb 24 07:43:48 JST 2023
[    0.000000] Machine model: Xunlong Orange Pi R1 Plus Lts
[    0.000000] efi: UEFI not found.
[    0.000000] NUMA: No NUMA configuration found
[    0.000000] NUMA: Faking a node at [mem 0x0000000000200000-0x000000003fffffff]
[    0.000000] NUMA: NODE_DATA [mem 0x3fdb9100-0x3fdbafff]
[    0.000000] Zone ranges:
[    0.000000]   DMA      [mem 0x0000000000200000-0x000000003fffffff]
[    0.000000]   DMA32    empty
[    0.000000]   Normal   empty
[    0.000000] Movable zone start for each node
[    0.000000] Early memory node ranges
[    0.000000]   node   0: [mem 0x0000000000200000-0x000000003fffffff]
[    0.000000] Initmem setup node 0 [mem 0x0000000000200000-0x000000003fffffff]
[    0.000000] On node 0 totalpages: 261632
[    0.000000]   DMA zone: 4088 pages used for memmap
[    0.000000]   DMA zone: 0 pages reserved
[    0.000000]   DMA zone: 261632 pages, LIFO batch:63
[    0.000000] cma: Reserved 128 MiB at 0x0000000035000000
[    0.000000] psci: probing for conduit method from DT.
[    0.000000] psci: PSCIv1.0 detected in firmware.
[    0.000000] psci: Using standard PSCI v0.2 function IDs
[    0.000000] psci: MIGRATE_INFO_TYPE not supported.
[    0.000000] psci: SMC Calling Convention v1.0
[    0.000000] percpu: Embedded 32 pages/cpu s93976 r8192 d28904 u131072
[    0.000000] pcpu-alloc: s93976 r8192 d28904 u131072 alloc=32*4096
[    0.000000] pcpu-alloc: [0] 0 [0] 1 [0] 2 [0] 3 
[    0.000000] Detected VIPT I-cache on CPU0
[    0.000000] CPU features: detected: ARM erratum 845719
[    0.000000] Built 1 zonelists, mobility grouping on.  Total pages: 257544
[    0.000000] Policy zone: DMA
[    0.000000] Kernel command line: root=UUID=caf840a6-547e-42ae-9a95-71bfd48afff1 rootwait rootfstype=ext4 console=ttyS2,1500000  consoleblank=0 loglevel=1 ubootpart=68cd18b9-01 usb-storage.quirks=0x2537:0x1066:u,0x2537:0x1068:u   cgroup_enable=cpuset cgroup_memory=1 cgroup_enable=memory swapaccount=1
[    0.000000] Dentry cache hash table entries: 131072 (order: 8, 1048576 bytes, linear)
[    0.000000] Inode-cache hash table entries: 65536 (order: 7, 524288 bytes, linear)
[    0.000000] mem auto-init: stack:off, heap alloc:on, heap free:off
[    0.000000] Memory: 851820K/1046528K available (14912K kernel code, 2632K rwdata, 5992K rodata, 4352K init, 580K bss, 63636K reserved, 131072K cma-reserved)
[    0.000000] SLUB: HWalign=64, Order=0-3, MinObjects=0, CPUs=4, Nodes=1
[    0.000000] rcu: Preemptible hierarchical RCU implementation.
[    0.000000] rcu: 	RCU event tracing is enabled.
[    0.000000] rcu: 	RCU restricting CPUs from NR_CPUS=256 to nr_cpu_ids=4.
[    0.000000] 	Trampoline variant of Tasks RCU enabled.
[    0.000000] 	Rude variant of Tasks RCU enabled.
[    0.000000] 	Tracing variant of Tasks RCU enabled.
[    0.000000] rcu: RCU calculated value of scheduler-enlistment delay is 25 jiffies.
[    0.000000] rcu: Adjusting geometry for rcu_fanout_leaf=16, nr_cpu_ids=4
[    0.000000] NR_IRQS: 64, nr_irqs: 64, preallocated irqs: 0
[    0.000000] GIC: Using split EOI/Deactivate mode
[    0.000000] random: get_random_bytes called from start_kernel+0x690/0x848 with crng_init=0
[    0.000000] arch_timer: cp15 timer(s) running at 24.00MHz (phys).
[    0.000000] clocksource: arch_sys_counter: mask: 0xffffffffffffff max_cycles: 0x588fe9dc0, max_idle_ns: 440795202592 ns
[    0.000008] sched_clock: 56 bits at 24MHz, resolution 41ns, wraps every 4398046511097ns
[    0.000902] Console: colour dummy device 80x25
[    0.001062] Calibrating delay loop (skipped), value calculated using timer frequency.. 48.00 BogoMIPS (lpj=96000)
[    0.001087] pid_max: default: 32768 minimum: 301
[    0.001266] LSM: Security Framework initializing
[    0.001329] Yama: becoming mindful.
[    0.001503] AppArmor: AppArmor initialized
[    0.001600] Mount-cache hash table entries: 2048 (order: 2, 16384 bytes, linear)
[    0.001626] Mountpoint-cache hash table entries: 2048 (order: 2, 16384 bytes, linear)
[    0.005226] rcu: Hierarchical SRCU implementation.
[    0.008485] EFI services will not be available.
[    0.009211] smp: Bringing up secondary CPUs ...
[    0.010301] Detected VIPT I-cache on CPU1
[    0.010409] CPU1: Booted secondary processor 0x0000000001 [0x410fd034]
[    0.011696] Detected VIPT I-cache on CPU2
[    0.011789] CPU2: Booted secondary processor 0x0000000002 [0x410fd034]
[    0.013199] Detected VIPT I-cache on CPU3
[    0.013293] CPU3: Booted secondary processor 0x0000000003 [0x410fd034]
[    0.013530] smp: Brought up 1 node, 4 CPUs
[    0.013550] SMP: Total of 4 processors activated.
[    0.013563] CPU features: detected: 32-bit EL0 Support
[    0.013576] CPU features: detected: CRC32 instructions
[    0.013589] CPU features: detected: 32-bit EL1 Support
[    0.035070] CPU: All CPU(s) started at EL2
[    0.035145] alternatives: patching kernel code
[    0.037789] devtmpfs: initialized
[    0.058942] Registered cp15_barrier emulation handler
[    0.058973] Registered setend emulation handler
[    0.059370] clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 7645041785100000 ns
[    0.059428] futex hash table entries: 1024 (order: 4, 65536 bytes, linear)
[    0.066270] pinctrl core: initialized pinctrl subsystem
[    0.067432] DMI not present or invalid.
[    0.068444] NET: Registered protocol family 16
[    0.072282] DMA: preallocated 2048 KiB GFP_KERNEL pool for atomic allocations
[    0.073135] DMA: preallocated 2048 KiB GFP_KERNEL|GFP_DMA pool for atomic allocations
[    0.074875] DMA: preallocated 2048 KiB GFP_KERNEL|GFP_DMA32 pool for atomic allocations
[    0.075084] audit: initializing netlink subsys (disabled)
[    0.075596] audit: type=2000 audit(0.072:1): state=initialized audit_enabled=0 res=1
[    0.077096] thermal_sys: Registered thermal governor 'fair_share'
[    0.077110] thermal_sys: Registered thermal governor 'bang_bang'
[    0.077121] thermal_sys: Registered thermal governor 'step_wise'
[    0.077132] thermal_sys: Registered thermal governor 'user_space'
[    0.077659] cpuidle: using governor menu
[    0.078218] hw-breakpoint: found 6 breakpoint and 4 watchpoint registers.
[    0.078433] ASID allocator initialised with 65536 entries
[    0.080475] Serial: AMBA PL011 UART driver
[    0.144961] HugeTLB registered 1.00 GiB page size, pre-allocated 0 pages
[    0.144983] HugeTLB registered 32.0 MiB page size, pre-allocated 0 pages
[    0.144994] HugeTLB registered 2.00 MiB page size, pre-allocated 0 pages
[    0.145007] HugeTLB registered 64.0 KiB page size, pre-allocated 0 pages
[    0.151991] cryptd: max_cpu_qlen set to 1000
[    0.233325] raid6: neonx8   gen()  1052 MB/s
[    0.301455] raid6: neonx8   xor()   780 MB/s
[    0.369603] raid6: neonx4   gen()  1077 MB/s
[    0.437748] raid6: neonx4   xor()   772 MB/s
[    0.505914] raid6: neonx2   gen()  1013 MB/s
[    0.574050] raid6: neonx2   xor()   718 MB/s
[    0.642200] raid6: neonx1   gen()   886 MB/s
[    0.710346] raid6: neonx1   xor()   610 MB/s
[    0.778507] raid6: int64x8  gen()   745 MB/s
[    0.846685] raid6: int64x8  xor()   392 MB/s
[    0.914789] raid6: int64x4  gen()   828 MB/s
[    0.982942] raid6: int64x4  xor()   418 MB/s
[    1.051082] raid6: int64x2  gen()   707 MB/s
[    1.119229] raid6: int64x2  xor()   365 MB/s
[    1.187371] raid6: int64x1  gen()   526 MB/s
[    1.255548] raid6: int64x1  xor()   279 MB/s
[    1.255559] raid6: using algorithm neonx4 gen() 1077 MB/s
[    1.255568] raid6: .... xor() 772 MB/s, rmw enabled
[    1.255578] raid6: using neon recovery algorithm
[    1.257034] reg-fixed-voltage sdmmc-regulator: Failed to register regulator: -517
[    1.260637] iommu: Default domain type: Translated 
[    1.262214] vgaarb: loaded
[    1.263159] SCSI subsystem initialized
[    1.263537] libata version 3.00 loaded.
[    1.264080] usbcore: registered new interface driver usbfs
[    1.264157] usbcore: registered new interface driver hub
[    1.264229] usbcore: registered new device driver usb
[    1.264875] pps_core: LinuxPPS API ver. 1 registered
[    1.264886] pps_core: Software ver. 5.3.6 - Copyright 2005-2007 Rodolfo Giometti <giometti@linux.it>
[    1.264913] PTP clock support registered
[    1.265173] EDAC MC: Ver: 3.0.0
[    1.267455] NetLabel: Initializing
[    1.267474] NetLabel:  domain hash size = 128
[    1.267482] NetLabel:  protocols = UNLABELED CIPSOv4 CALIPSO
[    1.267610] NetLabel:  unlabeled traffic allowed by default
[    1.268508] clocksource: Switched to clocksource arch_sys_counter
[    1.492956] VFS: Disk quotas dquot_6.6.0
[    1.493085] VFS: Dquot-cache hash table entries: 512 (order 0, 4096 bytes)
[    1.494630] AppArmor: AppArmor Filesystem Enabled
[    1.508480] NET: Registered protocol family 2
[    1.508800] IP idents hash table entries: 16384 (order: 5, 131072 bytes, linear)
[    1.510941] tcp_listen_portaddr_hash hash table entries: 512 (order: 1, 8192 bytes, linear)
[    1.511020] TCP established hash table entries: 8192 (order: 4, 65536 bytes, linear)
[    1.511304] TCP bind hash table entries: 8192 (order: 5, 131072 bytes, linear)
[    1.511501] TCP: Hash tables configured (established 8192 bind 8192)
[    1.511786] UDP hash table entries: 512 (order: 2, 16384 bytes, linear)
[    1.511853] UDP-Lite hash table entries: 512 (order: 2, 16384 bytes, linear)
[    1.512262] NET: Registered protocol family 1
[    1.512322] NET: Registered protocol family 44
[    1.512346] PCI: CLS 0 bytes, default 64
[    1.512870] Trying to unpack rootfs image as initramfs...
[    2.927842] Freeing initrd memory: 14176K
[    2.929925] hw perfevents: enabled with armv8_cortex_a53 PMU driver, 7 counters available
[    2.930535] kvm [1]: IPA Size Limit: 40 bits
[    2.932835] kvm [1]: vgic interrupt IRQ9
[    2.933107] kvm [1]: Hyp mode initialized successfully
[    2.947050] Initialise system trusted keyrings
[    2.947139] Key type blacklist registered
[    2.947523] workingset: timestamp_bits=44 max_order=18 bucket_order=0
[    2.958456] zbud: loaded
[    2.961511] squashfs: version 4.0 (2009/01/31) Phillip Lougher
[    2.962934] fuse: init (API version 7.32)
[    2.965285] integrity: Platform Keyring initialized
[    3.037582] xor: measuring software checksum speed
[    3.045722]    8regs           :  1217 MB/sec
[    3.052776]    32regs          :  1401 MB/sec
[    3.062066]    arm64_neon      :  1062 MB/sec
[    3.062077] xor: using function: 32regs (1401 MB/sec)
[    3.062100] Key type asymmetric registered
[    3.062111] Asymmetric key parser 'x509' registered
[    3.062213] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 247)
[    3.062509] io scheduler mq-deadline registered
[    3.062520] io scheduler kyber registered
[    3.062784] io scheduler bfq registered
[    3.068792] rockchip-u3phy ff470000.usb3-phy: vbus_drv is not assigned
[    3.071621] rockchip-u3phy ff470000.usb3-phy: Rockchip u3phy initialized successfully
[    3.086323] dma-pl330 ff1f0000.dmac: Loaded driver for PL330 DMAC-241330
[    3.086348] dma-pl330 ff1f0000.dmac: 	DBUFF-128x8bytes Num_Chans-8 Num_Peri-20 Num_Events-16
[    3.091674] Serial: 8250/16550 driver, 8 ports, IRQ sharing disabled
[    3.096801] printk: console [ttyS2] disabled
[    3.096943] ff130000.serial: ttyS2 at MMIO 0xff130000 (irq = 20, base_baud = 1500000) is a 16550A
[    3.097215] printk: console [ttyS2] enabled
[    3.099080] Serial: AMBA driver
[    3.121647] loop: module loaded
[    3.128977] spi-nor spi0.0: zb25vq128 (16384 Kbytes)
[    3.152935] libphy: Fixed MDIO Bus: probed
[    3.153971] tun: Universal TUN/TAP device driver, 1.6
[    3.155222] thunder_xcv, ver 1.0
[    3.155303] thunder_bgx, ver 1.0
[    3.155389] nicpf, ver 1.0
[    3.156236] e1000e: Intel(R) PRO/1000 Network Driver
[    3.156247] e1000e: Copyright(c) 1999 - 2015 Intel Corporation.
[    3.156340] igb: Intel(R) Gigabit Ethernet Network Driver
[    3.156348] igb: Copyright (c) 2007-2014 Intel Corporation.
[    3.156412] igbvf: Intel(R) Gigabit Virtual Function Network Driver
[    3.156421] igbvf: Copyright (c) 2009 - 2012 Intel Corporation.
[    3.156758] sky2: driver version 1.30
[    3.157588] VFIO - User Level meta-driver version: 0.3
[    3.164970] dwc2 ff580000.usb: supply vusb_d not found, using dummy regulator
[    3.165223] dwc2 ff580000.usb: supply vusb_a not found, using dummy regulator
[    3.292617] dwc2 ff580000.usb: EPs: 10, dedicated fifos, 972 entries in SPRAM
[    3.293206] dwc2 ff580000.usb: DWC OTG Controller
[    3.293254] dwc2 ff580000.usb: new USB bus registered, assigned bus number 1
[    3.293325] dwc2 ff580000.usb: irq 37, io mem 0xff580000
[    3.293667] usb usb1: New USB device found, idVendor=1d6b, idProduct=0002, bcdDevice= 5.10
[    3.293683] usb usb1: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    3.293696] usb usb1: Product: DWC OTG Controller
[    3.293710] usb usb1: Manufacturer: Linux 5.10.44-rockchip64 dwc2_hsotg
[    3.293721] usb usb1: SerialNumber: ff580000.usb
[    3.294774] hub 1-0:1.0: USB hub found
[    3.294838] hub 1-0:1.0: 1 port detected
[    3.297406] ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
[    3.297471] ehci-pci: EHCI PCI platform driver
[    3.297549] ehci-platform: EHCI generic platform driver
[    3.300331] ehci-platform ff5c0000.usb: EHCI Host Controller
[    3.300374] ehci-platform ff5c0000.usb: new USB bus registered, assigned bus number 2
[    3.300918] ehci-platform ff5c0000.usb: irq 38, io mem 0xff5c0000
[    3.316538] ehci-platform ff5c0000.usb: USB 2.0 started, EHCI 1.00
[    3.316954] usb usb2: New USB device found, idVendor=1d6b, idProduct=0002, bcdDevice= 5.10
[    3.316970] usb usb2: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    3.316984] usb usb2: Product: EHCI Host Controller
[    3.316996] usb usb2: Manufacturer: Linux 5.10.44-rockchip64 ehci_hcd
[    3.317009] usb usb2: SerialNumber: ff5c0000.usb
[    3.317955] hub 2-0:1.0: USB hub found
[    3.318020] hub 2-0:1.0: 1 port detected
[    3.319003] ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
[    3.319057] ohci-pci: OHCI PCI platform driver
[    3.319162] ohci-platform: OHCI generic platform driver
[    3.319859] ohci-platform ff5d0000.usb: Generic Platform OHCI controller
[    3.319907] ohci-platform ff5d0000.usb: new USB bus registered, assigned bus number 3
[    3.320195] ohci-platform ff5d0000.usb: irq 39, io mem 0xff5d0000
[    3.380826] usb usb3: New USB device found, idVendor=1d6b, idProduct=0001, bcdDevice= 5.10
[    3.380846] usb usb3: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    3.380859] usb usb3: Product: Generic Platform OHCI controller
[    3.380871] usb usb3: Manufacturer: Linux 5.10.44-rockchip64 ohci_hcd
[    3.380885] usb usb3: SerialNumber: ff5d0000.usb
[    3.381819] hub 3-0:1.0: USB hub found
[    3.381886] hub 3-0:1.0: 1 port detected
[    3.383808] xhci-hcd xhci-hcd.0.auto: xHCI Host Controller
[    3.383855] xhci-hcd xhci-hcd.0.auto: new USB bus registered, assigned bus number 4
[    3.384142] xhci-hcd xhci-hcd.0.auto: hcc params 0x0220fe64 hci version 0x110 quirks 0x0000000002010010
[    3.384266] xhci-hcd xhci-hcd.0.auto: irq 46, io mem 0xff600000
[    3.385083] usb usb4: New USB device found, idVendor=1d6b, idProduct=0002, bcdDevice= 5.10
[    3.385100] usb usb4: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    3.385114] usb usb4: Product: xHCI Host Controller
[    3.385126] usb usb4: Manufacturer: Linux 5.10.44-rockchip64 xhci-hcd
[    3.385138] usb usb4: SerialNumber: xhci-hcd.0.auto
[    3.386058] hub 4-0:1.0: USB hub found
[    3.386123] hub 4-0:1.0: 1 port detected
[    3.386741] xhci-hcd xhci-hcd.0.auto: xHCI Host Controller
[    3.386783] xhci-hcd xhci-hcd.0.auto: new USB bus registered, assigned bus number 5
[    3.386815] xhci-hcd xhci-hcd.0.auto: Host supports USB 3.0 SuperSpeed
[    3.386948] usb usb5: We don't know the algorithms for LPM for this host, disabling LPM.
[    3.387177] usb usb5: New USB device found, idVendor=1d6b, idProduct=0003, bcdDevice= 5.10
[    3.387194] usb usb5: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    3.387207] usb usb5: Product: xHCI Host Controller
[    3.387219] usb usb5: Manufacturer: Linux 5.10.44-rockchip64 xhci-hcd
[    3.387231] usb usb5: SerialNumber: xhci-hcd.0.auto
[    3.388098] hub 5-0:1.0: USB hub found
[    3.388161] hub 5-0:1.0: 1 port detected
[    3.389331] usbcore: registered new interface driver usb-storage
[    3.391718] mousedev: PS/2 mouse device common for all mice
[    3.393275] i2c /dev entries driver
[    3.398954] rk808 1-0018: chip id: 0x8050
[    3.406974] rk808-regulator rk808-regulator: there is no dvs0 gpio
[    3.407028] rk808-regulator rk808-regulator: there is no dvs1 gpio
[    3.407044] rk808-regulator rk808-regulator: max buck steps per change: 8
[    3.409506] vdd_logic: supplied by vcc_sys
[    3.411982] vdd_arm: supplied by vcc_sys
[    3.412537] vcc_ddr: supplied by vcc_sys
[    3.413970] vcc_io: supplied by vcc_sys
[    3.416317] vcc_18: supplied by vcc_io
[    3.420916] vcc18_emmc: supplied by vcc_io
[    3.425530] vdd_10: supplied by vcc_io
[    3.439263] rk808-rtc rk808-rtc: registered as rtc0
[    3.441057] rk808-rtc rk808-rtc: setting system clock to 2023-02-24T07:52:28 UTC (1677225148)
[    3.443395] input: rk805 pwrkey as /devices/platform/ff160000.i2c/i2c-1/1-0018/rk805-pwrkey/input/input0
[    3.447099] rockchip-thermal ff250000.tsadc: Missing tshut mode property, using default (cru)
[    3.447125] rockchip-thermal ff250000.tsadc: Missing tshut-polarity property, using default (low)
[    3.449359] dw_wdt ff1a0000.watchdog: No valid TOPs array specified
[    3.452245] sdhci: Secure Digital Host Controller Interface driver
[    3.452261] sdhci: Copyright(c) Pierre Ossman
[    3.452312] Synopsys Designware Multimedia Card Interface Driver
[    3.453374] sdhci-pltfm: SDHCI platform and OF driver helper
[    3.454224] dwmmc_rockchip ff500000.mmc: IDMAC supports 32-bit address mode.
[    3.454277] dwmmc_rockchip ff500000.mmc: Using internal DMA controller.
[    3.454297] dwmmc_rockchip ff500000.mmc: Version ID is 270a
[    3.454405] dwmmc_rockchip ff500000.mmc: DW MMC controller at irq 35,32 bit host data width,256 deep fifo
[    3.456772] ledtrig-cpu: registered to indicate activity on CPUs
[    3.457888] hid: raw HID events driver (C) Jiri Kosina
[    3.458156] usbcore: registered new interface driver usbhid
[    3.458165] usbhid: USB HID core driver
[    3.463708] drop_monitor: Initializing network drop monitor service
[    3.465115] NET: Registered protocol family 10
[    3.519523] Segment Routing with IPv6
[    3.519694] NET: Registered protocol family 17
[    3.519959] 8021q: 802.1Q VLAN Support v1.8
[    3.520063] Key type dns_resolver registered
[    3.521181] registered taskstats version 1
[    3.521209] Loading compiled-in X.509 certificates
[    3.527183] Loaded X.509 cert 'Build time autogenerated kernel key: a893bf0605f82fd245d93c76e8d6ca7800a7413d'
[    3.532969] zswap: loaded using pool zstd/z3fold
[    3.533861] Key type ._fscrypt registered
[    3.533878] Key type .fscrypt registered
[    3.533887] Key type fscrypt-provisioning registered
[    3.538186] Btrfs loaded, crc32c=crc32c-generic
[    3.564251] Key type encrypted registered
[    3.564296] AppArmor: AppArmor sha1 policy hashing enabled
[    3.614778] friendlyelec-board board: Serial		: e321813e2b5ba4ed
[    3.616089] vcc_sd: supplied by vcc_io
[    3.623039] rk3328-dmc-freq dmc: current ATF version 0x101
[    3.623324] dwmmc_rockchip ff500000.mmc: IDMAC supports 32-bit address mode.
[    3.623368] dwmmc_rockchip ff500000.mmc: Using internal DMA controller.
[    3.623388] dwmmc_rockchip ff500000.mmc: Version ID is 270a
[    3.623452] dwmmc_rockchip ff500000.mmc: DW MMC controller at irq 35,32 bit host data width,256 deep fifo
[    3.628654] input: gpio-keys as /devices/platform/gpio-keys/input/input1
[    3.629634] of_cfs_init
[    3.629714] of_cfs_init: OK
[    3.631588] dw-apb-uart ff130000.serial: forbid DMA for kernel console
[    3.642968] mmc_host mmc0: Bus speed (slot 0) = 400000Hz (slot req 400000Hz, actual 400000HZ div = 0)
[    3.660382] Freeing unused kernel memory: 4352K
[    3.660634] Run /init as init process
[    3.660646]   with arguments:
[    3.660655]     /init
[    3.660664]   with environment:
[    3.660675]     HOME=/
[    3.660683]     TERM=linux
[    3.660694]     ubootpart=68cd18b9-01
[    3.660703]     cgroup_enable=memory
[    3.660712]     cgroup_memory=1
[    3.666052] random: fast init done
[    3.745940] mmc_host mmc0: Bus speed (slot 0) = 150000000Hz (slot req 150000000Hz, actual 150000000HZ div = 0)
[    4.023575] dwmmc_rockchip ff500000.mmc: Successfully tuned phase to 188
[    4.023643] mmc0: new ultra high speed SDR104 SDHC card at address aaaa
[    4.028303] mmcblk0: mmc0:aaaa SL32G 29.7 GiB 
[    4.035906]  mmcblk0: p1
[    4.512022] gpio-syscon ff100000.syscon:grf-gpio: can't read the data register offset!
[    4.721735] rk_gmac-dwmac ff540000.ethernet: IRQ eth_wake_irq not found
[    4.721760] rk_gmac-dwmac ff540000.ethernet: IRQ eth_lpi not found
[    4.722047] rk_gmac-dwmac ff540000.ethernet: PTP uses main clock
[    4.722586] rk_gmac-dwmac ff540000.ethernet: clock input or output? (input).
[    4.722617] rk_gmac-dwmac ff540000.ethernet: TX delay(0x19).
[    4.722632] rk_gmac-dwmac ff540000.ethernet: RX delay(0x5).
[    4.722661] rk_gmac-dwmac ff540000.ethernet: integrated PHY? (no).
[    4.722792] rk_gmac-dwmac ff540000.ethernet: cannot get clock clk_mac_speed
[    4.722804] rk_gmac-dwmac ff540000.ethernet: clock input from PHY
[    4.728725] rk_gmac-dwmac ff540000.ethernet: init for RGMII
[    4.729506] rk_gmac-dwmac ff540000.ethernet: User ID: 0x10, Synopsys ID: 0x35
[    4.729536] rk_gmac-dwmac ff540000.ethernet: 	DWMAC1000
[    4.729551] rk_gmac-dwmac ff540000.ethernet: DMA HW capability register supported
[    4.729563] rk_gmac-dwmac ff540000.ethernet: RX Checksum Offload Engine supported
[    4.729574] rk_gmac-dwmac ff540000.ethernet: COE Type 2
[    4.729584] rk_gmac-dwmac ff540000.ethernet: TX Checksum insertion supported
[    4.729594] rk_gmac-dwmac ff540000.ethernet: Wake-Up On Lan supported
[    4.729843] rk_gmac-dwmac ff540000.ethernet: Normal descriptors
[    4.729861] rk_gmac-dwmac ff540000.ethernet: Ring mode enabled
[    4.729873] rk_gmac-dwmac ff540000.ethernet: Enable RX Mitigation via HW Watchdog Timer
[    4.817725] libphy: stmmac: probed
[    5.563533] EXT4-fs (mmcblk0p1): mounted filesystem with writeback data mode. Opts: (null)
[    5.736799] usb 5-1: new SuperSpeed Gen 1 USB device number 2 using xhci-hcd
[    5.758585] usb 5-1: New USB device found, idVendor=0bda, idProduct=8153, bcdDevice=31.00
[    5.758608] usb 5-1: New USB device strings: Mfr=1, Product=2, SerialNumber=6
[    5.758622] usb 5-1: Product: USB 10/100/1000 LAN
[    5.758633] usb 5-1: Manufacturer: Realtek
[    5.758645] usb 5-1: SerialNumber: 001000001
[    6.201178] systemd[1]: Inserted module 'autofs4'
[    6.277003] systemd[1]: systemd 245.4-4ubuntu3.19 running in system mode. (+PAM +AUDIT +SELINUX +IMA +APPARMOR +SMACK +SYSVINIT +UTMP +LIBCRYPTSETUP +GCRYPT +GNUTLS +ACL +XZ +LZ4 +SECCOMP +BLKID +ELFUTILS +KMOD +IDN2 -IDN +PCRE2 default-hierarchy=hybrid)
[    6.278377] systemd[1]: Detected architecture arm64.
[    6.311803] systemd[1]: Set hostname to <orangepir1plus-lts>.
[    7.193617] random: systemd: uninitialized urandom read (16 bytes read)
[    7.201134] systemd[1]: Created slice system-modprobe.slice.
[    7.212860] random: systemd: uninitialized urandom read (16 bytes read)
[    7.215590] systemd[1]: Created slice system-serial\x2dgetty.slice.
[    7.216946] random: systemd: uninitialized urandom read (16 bytes read)
[    7.219585] systemd[1]: Created slice User and Session Slice.
[    7.221740] systemd[1]: Started Dispatch Password Requests to Console Directory Watch.
[    7.233403] systemd[1]: Started Forward Password Requests to Wall Directory Watch.
[    7.246545] systemd[1]: Set up automount Arbitrary Executable File Formats File System Automount Point.
[    7.257182] systemd[1]: Reached target Local Encrypted Volumes.
[    7.269094] systemd[1]: Reached target Remote File Systems.
[    7.280893] systemd[1]: Reached target Slices.
[    7.292937] systemd[1]: Reached target Swap.
[    7.304903] systemd[1]: Reached target System Time Set.
[    7.307118] systemd[1]: Listening on Syslog Socket.
[    7.317954] systemd[1]: Listening on fsck to fsckd communication Socket.
[    7.329506] systemd[1]: Listening on initctl Compatibility Named Pipe.
[    7.342743] systemd[1]: Listening on Journal Audit Socket.
[    7.345051] systemd[1]: Listening on Journal Socket (/dev/log).
[    7.358192] systemd[1]: Listening on Journal Socket.
[    7.370160] systemd[1]: Listening on udev Control Socket.
[    7.372227] systemd[1]: Listening on udev Kernel Socket.
[    7.383339] systemd[1]: Mounting Huge Pages File System...
[    7.403169] systemd[1]: Mounting POSIX Message Queue File System...
[    7.415534] systemd[1]: Mounting Kernel Debug File System...
[    7.437740] systemd[1]: Mounting Kernel Trace File System...
[    7.465718] systemd[1]: Starting Restore / save the current clock...
[    7.477050] systemd[1]: Starting Set the console keyboard layout...
[    7.491431] systemd[1]: Starting Create list of static device nodes for the current kernel...
[    7.516796] systemd[1]: Starting Load Kernel Module chromeos_pstore...
[    7.531790] systemd[1]: Starting Load Kernel Module drm...
[    7.533869] systemd[1]: Condition check resulted in Load Kernel Module efi_pstore being skipped.
[    7.546476] systemd[1]: Starting Load Kernel Module pstore_blk...
[    7.560619] systemd[1]: Starting Load Kernel Module pstore_zone...
[    7.575035] systemd[1]: Starting Load Kernel Module ramoops...
[    7.598817] systemd[1]: Started Nameserver information manager.
[    7.602169] systemd[1]: Reached target Network (Pre).
[    7.616933] systemd[1]: Condition check resulted in Set Up Additional Binary Formats being skipped.
[    7.617305] systemd[1]: Condition check resulted in File System Check on Root Device being skipped.
[    7.636007] systemd[1]: Starting Load Kernel Modules...
[    7.659644] systemd[1]: Starting Remount Root and Kernel File Systems...
[    7.684225] systemd[1]: Starting udev Coldplug all Devices...
[    7.718759] systemd[1]: Mounted Huge Pages File System.
[    7.722183] systemd[1]: Mounted POSIX Message Queue File System.
[    7.733129] EXT4-fs (mmcblk0p1): re-mounted. Opts: commit=600,errors=remount-ro
[    7.741518] systemd[1]: Mounted Kernel Debug File System.
[    7.745600] systemd[1]: Mounted Kernel Trace File System.
[    7.753955] systemd[1]: Finished Restore / save the current clock.
[    7.767207] g_serial gadget: Gadget Serial v2.4
[    7.767231] g_serial gadget: g_serial ready
[    7.767251] dwc2 ff580000.usb: bound driver g_serial
[    7.772789] systemd[1]: Finished Create list of static device nodes for the current kernel.
[    7.788053] systemd[1]: modprobe@chromeos_pstore.service: Succeeded.
[    7.794354] systemd[1]: Finished Load Kernel Module chromeos_pstore.
[    7.808803] systemd[1]: modprobe@drm.service: Succeeded.
[    7.813955] systemd[1]: Finished Load Kernel Module drm.
[    7.818253] systemd[1]: modprobe@pstore_blk.service: Succeeded.
[    7.823111] systemd[1]: Finished Load Kernel Module pstore_blk.
[    7.835809] systemd[1]: modprobe@pstore_zone.service: Succeeded.
[    7.840948] systemd[1]: Finished Load Kernel Module pstore_zone.
[    7.855812] systemd[1]: modprobe@ramoops.service: Succeeded.
[    7.860055] systemd[1]: Finished Load Kernel Module ramoops.
[    7.874754] systemd[1]: Finished Load Kernel Modules.
[    7.895351] systemd[1]: Finished Remount Root and Kernel File Systems.
[    7.916880] systemd[1]: Mounting FUSE Control File System...
[    7.938889] systemd[1]: Mounting Kernel Configuration File System...
[    7.946645] systemd[1]: Condition check resulted in Rebuild Hardware Database being skipped.
[    7.947270] systemd[1]: Condition check resulted in Platform Persistent Storage Archival being skipped.
[    7.958165] systemd[1]: Starting Load/Save Random Seed...
[    7.979544] systemd[1]: Starting Apply Kernel Variables...
[    8.017023] systemd[1]: Starting Create System Users...
[    8.058246] systemd[1]: Mounted FUSE Control File System.
[    8.063083] systemd[1]: Mounted Kernel Configuration File System.
[    8.099606] systemd[1]: Finished Create System Users.
[    8.121362] systemd[1]: Starting Create Static Device Nodes in /dev...
[    8.131641] systemd[1]: Finished Apply Kernel Variables.
[    8.198206] systemd[1]: Finished Set the console keyboard layout.
[    8.215645] systemd[1]: Finished Create Static Device Nodes in /dev.
[    8.230448] systemd[1]: Reached target Local File Systems (Pre).
[    8.253172] systemd[1]: Mounting /tmp...
[    8.275793] systemd[1]: Starting udev Kernel Device Manager...
[    8.293742] systemd[1]: Mounted /tmp.
[    8.310228] systemd[1]: Reached target Local File Systems.
[    8.321935] systemd[1]: Starting Set console font and keymap...
[    8.347074] systemd[1]: Starting Orange Pi ZRAM config...
[    8.357471] systemd[1]: Condition check resulted in Commit a transient machine-id on disk being skipped.
[    8.373415] systemd[1]: Finished Set console font and keymap.
[    8.515077] systemd[1]: Started udev Kernel Device Manager.
[    8.569418] systemd[1]: Finished udev Coldplug all Devices.
[    8.592365] systemd[1]: Starting Helper to synchronize boot up for ifupdown...
[    8.616030] systemd[1]: Found device /dev/ttyGS0.
[    8.637907] systemd[1]: Finished Helper to synchronize boot up for ifupdown.
[    8.658796] systemd[1]: Starting Raise network interfaces...
[    8.730459] zram: Added device: zram0
[    8.732315] zram: Added device: zram1
[    8.734319] zram: Added device: zram2
[    8.860372] zram1: detected capacity change from 0 to 512729088
[    9.183852] systemd[1]: Finished Raise network interfaces.
[    9.482641] systemd[1]: Found device /dev/ttyS2.
[    9.899681] usbcore: registered new interface driver r8152
[    9.941322] usbcore: registered new interface driver cdc_ether
[    9.960682] Adding 500708k swap on /dev/zram1.  Priority:5 extents:1 across:500708k SSFS
[   10.075580] usb 5-1: reset SuperSpeed Gen 1 USB device number 2 using xhci-hcd
[   10.132191] zram0: detected capacity change from 0 to 52428800
[   10.170047] r8152 5-1:1.0 eth1: v2.14.0 (2020/09/24)
[   10.170064] r8152 5-1:1.0 eth1: This product is covered by one or more of the following patents:
               		US6,570,884, US6,115,776, and US6,327,625.

[   10.211751] r8152 5-1:1.0 lan0: renamed from eth1
[   10.272607] random: crng init done
[   10.272635] random: 7 urandom warning(s) missed due to ratelimiting
[   10.293266] systemd[1]: Finished Load/Save Random Seed.
[   10.296075] systemd[1]: Condition check resulted in Store a System Token in an EFI Variable being skipped.
[   10.319938] systemd[1]: Finished Orange Pi ZRAM config.
[   10.339159] systemd[1]: Starting Orange Pi memory supported logging...
[   10.423187] EXT4-fs (zram0): mounted filesystem without journal. Opts: discard
[   10.423243] ext4 filesystem being mounted at /var/log supports timestamps until 2038 (0x7fffffff)
[   13.641937] systemd[1]: Finished Orange Pi memory supported logging.
[   13.659578] systemd[1]: Starting Journal Service...
[   13.907045] systemd[1]: Started Journal Service.
[   13.961949] systemd-journald[551]: Received client request to flush runtime journal.
[   15.611940] yzhang..read phyaddr=0, phyid=4f51e91b
[   15.611964] yzhang..get YT8511, abt to set 125m clk out, phyaddr=0, phyid=4f51e91b
[   15.824593] yt8511_config_out_125m, phy clk out, val=0x008006
[   15.824871] yzhang..8511 set 125m clk out, reg=0x8006
[   15.824887] phy_yt8531_led_fixup in
[   15.827188] rk_gmac-dwmac ff540000.ethernet eth0: PHY [stmmac-0:00] driver [YT8531 Gigabit Ethernet] (irq=POLL)
[   15.852635] rk_gmac-dwmac ff540000.ethernet eth0: No Safety Features support found
[   15.852671] rk_gmac-dwmac ff540000.ethernet eth0: PTP not supported by HW
[   15.853416] rk_gmac-dwmac ff540000.ethernet eth0: configuring for phy/rgmii link mode
[   16.607999] IPv6: ADDRCONF(NETDEV_CHANGE): lan0: link becomes ready
[   16.609599] r8152 5-1:1.0 lan0: carrier on

```



## Supported boards

Soc | Boards |
|:--|:--|
| Allwinner H2+ | Orange Pi Zero/R1 |
| Allwinner H3 | Orange Pi One/Lite/Pc/PcPlus/Plus/Plus2E/ZeroPlus2 | 
| Allwinner H5 | Orange Pi Pc2/Prime/ZeroPlus/ZeroPlus2| 
| Allwinner H6 | Orange Pi 3/3 LTS/Lite2/OnePlus| 
| Allwinner H616 | Orange Pi Zero2 | 
| Rockchip RK3328 | Orange Pi R1Plus/R1Plus LTS| 
| Rockchip RK3399 | Orange Pi 4/4B | 

## Download links

- 中文链接：     http://www.orangepi.cn
- English link：http://www.orangepi.org
