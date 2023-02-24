for Orange Pi R1 Plus LTS on Wsl(jammy and docker) environment

./output/images/Orangepir1plus-lts_2.2.2_ubuntu_focal_server_linux5.10.44_minimal/Orangepir1plus-lts_2.2.2_ubuntu_focal_server_linux5.10.44_minimal.img

<img width="731" alt="スクリーンショット 2023-02-24 134906" src="https://user-images.githubusercontent.com/59951021/221100023-44c8a493-4e29-4c61-a815-03446ceeb48c.png">

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
