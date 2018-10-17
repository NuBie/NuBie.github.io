---
layout: post
title:  Oreo kernel for mido 
date:   2018-09-01 00:55:00 +0700
categories: guzzo tips
---
Ini adalah changelog perubahan Kernel mido v3.18.y based on caf untuk Android Oreo Treble yang telah di merged ke github repository ! sources dapat dilihat [Disini!](https://github.com/NuBie/android_kernel_xiaomi_msm8953) dan untuk melihat malam minggu dev silahkan [klik ini !](https://raw.githubusercontent.com/NuBie/NuBie.github.io/master/__images/blob/001.png)

Changelog/Tracking :
---
*   --common kernel--
*   549129f add mdss idle state node
*   15d8164 remove mdss partial update region delays
*   0ce58b1 binder upstream
*   ede7958 Print vulkan memory types as well
*   cf8ca18 do not invoke loading of gpu zap shader
*   f927aba remove incorrect check to cap ab vote to ib vote
*   094135f fix mdss dsi potential buffer overflow
*   31cd970 sched/core: Properly fix constant logical operand Clang warning
*   b40f59c ALSA: rawmidi: Undo my 3.18.117 resolution
*   884706d fix memory leak free binder memory on error
*   255fb0e disable mdss xlog panic on error
*   3419350 msm: ipa3: Fix redundant wakelock releases in error paths
*   a04b05b workqueue: fix permissions for power-efficient_wq
*   068d846 UPSTREAM: fs/sync.c: remove unnecessary NULL f_mapping check in sync_file_range
*   649ca46 USB: f_fs: change wait as freezable
*   073cd30 cpufreq: Restore policy min/max limits on CPU online
*   62f2d1d arm64: Use optimized memcmp
*   413cac9 cpufreq: conservative: unlock sample_rate
*   69ef113 cpufreq: conservative: Decrease frequency faster when the timer deferred
*   bd83429 msm: mdss: update mdss perf when changing refresh rate
*   037a9fb prevent false check on qcom cpufreq
*   edd4158 Add USB HID gadget suport
*   12c0428 Makefile: fix segfaults when compiled with Clang
*   1e09dab Revert "sched: qhmp: avoid scheduling RT threads on cores currently handling softirqs"
*   d49bbe2 msm: kgsl: Remove POPP
*   ab889b6 msm: kgsl: Wake GPU upon receiving an ioctl rather than upon touch input

---
    ***********************************2018-10-18***********************************

---

0159397 staging: ion: msm: Apply d82ad70e8aff to msm_ion_custom_ioctl
8d1d648 BACKPORT: staging: android: ion: Pull out ion ioctls to a separate file
2c6bd49 Merge branch 'linux-3.18.y' of https://git.kernel.org/pub/scm/linux/kern
0d63979 Linux 3.18.124
ab94214 ebtables: arpreply: Add the standard target sanity check
72c6877 ubifs: Check for name being NULL while mounting
e289e19 cgroup: Fix deadlock in cpu hotplug path
4faa558 ext4: avoid running out of journal credits when appending to an inline f
5241002 jbd2: don't mark block as modified if the handle is out of credits
292dc96 ext4: add more inode number paranoia checks
fd26343 ext4: never move the system.data xattr out of the inode body
f8b8db0 ext4: always verify the magic number in xattr blocks
912e35d ext4: add corruption check in ext4_xattr_set_entry()
5141d33 ext4: fix false negatives *and* false positives in ext4_check_descriptor
6f6da33 ext4: always check block group bounds in ext4_init_block_bitmap()
08b1fd2 ext4: fix check to prevent initializing reserved inodes
8d41974 ext4: only look at the bg_flags field if it is valid
974abf8 USB: serial: simple: add Motorola Tetra MTP6550 id
d9e61bd PM / core: Clear the direct_complete flag on errors
726063c mac80211: fix setting IEEE80211_KEY_FLAG_RX_MGMT for AP mode keys
8858d0c PCI: Reprogram bridge prefetch registers on resume
b1f378d x86/vdso: Fix vDSO syscall fallback asm constraint regression
430d094 x86/vdso: Fix asm constraints on vDSO syscall fallbacks
39e616e fbdev/omapfb: fix omapfb_memory_read infoleak
ea20fab proc: restrict kernel stack dumps to root
01f7e02 mtd: fsl-quadspi: fix macro collision problems with READ/WRITE
685adc7 Make file credentials available to the seqfile interfaces
8c6fbba dm thin metadata: fix __udivdi3 undefined on 32-bit
1c07a7c ocfs2: fix locking for res->tracking and dlm->tracking_list
1b42ccd crypto: mxs-dcp - Fix wait logic on chan threads
ada05f7 smb2: fix missing files in root share directory listing
b4f13b6 xen: fix GCC warning and remove duplicate EVTCHN_ROW/EVTCHN_COL usage
f1cf612 xen/manage: don't complain about an empty value in control/sysrq node
fd51d7c cifs: read overflow in is_valid_oplock_break()
50997bd s390/qeth: don't dump past end of unknown HW header
f56aa68 r8169: Clear RTL_FLAG_TASK_*_PENDING when clearing RTL_FLAG_TASK_ENABLED
43f67da hexagon: modify ffs() and fls() to return int
ece6546 arch/hexagon: fix kernel/dma.c build warning
b438753 dm thin metadata: try to avoid ever aborting transactions
699c477 fs/cifs: suppress a string overflow warning
8c44ff3 USB: yurex: Check for truncation in yurex_read()
d90c014 RDMA/ucma: check fd type in ucma_migrate_id()
e467ada mm: madvise(MADV_DODUMP): allow hugetlbfs pages
792de67 tools/vm/page-types.c: fix "defined but not used" warning
2579073 tools/vm/slabinfo.c: fix sign-compare warning
15ace34 mac80211: shorten the IBSS debug messages
3655a53 mac80211: Fix station bandwidth setting after channel switch
869ce9b mac80211: fix a race between restart and CSA flows
33865da fs/cifs: don't translate SFM_SLASH (U+F026) to backslash
1ed8736 net: cadence: Fix a sleep-in-atomic-context bug in macb_halt_tx()
3f5fc65 RAID10 BUG_ON in raise_barrier when force is true and conf->barrier is 0
5f2da71 cfg80211: nl80211_update_ft_ies() to validate NL80211_ATTR_IE
9f91fbe gpio: adp5588: Fix sleep-in-atomic-context bug
44e7dfa mac80211: correct use of IEEE80211_VHT_CAP_RXSTBC_X
0a76f11 KVM: PPC: Book3S HV: Don't truncate HPTE index in xlate function
10c134d media: v4l: event: Prevent freeing event subscriptions while accessed
a46148c arm64: KVM: Sanitize PSTATE.M when being set from userspace
4e249d0 hwmon: (adt7475) Make adt7475_read_word() return errors
666a305 e1000: ensure to free old tx/rx rings in set_ringparam()
aa7ef1e e1000: check on netif_running() before calling e1000_up()
4aee595 thermal: of-thermal: disable passive polling when thermal zone is disabl
6836260 ext4: verify the depth of extent tree in ext4_find_extent()
d26e091 arm64: KVM: Tighten guest core register access from userspace
d82ad70 staging: android: ion: fix ION_IOC_{MAP,SHARE} use-after-free
be6f6ea scsi: target: iscsi: Use bin2hex instead of a re-implementation
05bebb4 USB: remove LPM management from usb_driver_claim_interface()
f309693 Revert "usb: cdc-wdm: Fix a sleep-in-atomic-context bug in service_outst
24e5fc9 USB: usbdevfs: restore warning for nonsensical flags
2ea0147 USB: usbdevfs: sanitize flags more
530d537 media: uvcvideo: Support realtek's UVC 1.5 device
843b66c slub: make ->cpu_partial unsigned int
48ba1bb USB: handle NULL config in usb_find_alt_setting()
75e71d4 USB: fix error handling in usb_driver_claim_interface()
6ea058b spi: rspi: Fix interrupted DMA transfers
5a5b2a2 spi: sh-msiof: Fix handling of write value for SISTR register
f4da70b spi: tegra20-slink: explicitly enable/disable clock
784a10d serial: cpm_uart: return immediately from console poll
0facefd floppy: Do not copy a kernel pointer to user memory in FDGETPRM ioctl
0fb40f7 nfsd: fix corrupted reply to badly ordered compound
5199f51 module: exclude SHN_UNDEF symbols from kallsyms api
8e74d31 ASoC: dapm: Fix potential DAI widget pointer deref when linking DAIs
b4bc21f scsi: bnx2i: add error handling for ioremap_nocache
fafbfb1 HID: hid-ntrig: add error handling for sysfs_create_group
d02f965 ARM: mvebu: declare asm symbols as character arrays in pmsu.c
cbc56a1 wlcore: Add missing PM call for wlcore_cmd_wait_for_event_or_timeout()
1ae2ccc rndis_wlan: potential buffer overflow in rndis_wlan_auth_indication()
ebfb72d ALSA: hda: Add AZX_DCAPS_PM_RUNTIME for AMD Raven Ridge
f228654 media: tm6000: add error handling for dvb_register_adapter
7376ca3 drivers/tty: add error handling for pcmcia_loop_config
59c5b0c staging: android: ashmem: Fix mmap size validation
4e8a8b0 media: soc_camera: ov772x: correct setting of banding filter
359c08d media: s3c-camif: ignore -ENOIOCTLCMD from v4l2_subdev_call for s_power
65ec1f1 ALSA: snd-aoa: add of_node_put() in error path
8963aa5 s390/extmem: fix gcc 8 stringop-overflow warning
f497869 alarmtimer: Prevent overflow for relative nanosleep
5c25cf1 usb: wusbcore: security: cast sizeof to int for comparison
f5ba827 scsi: ibmvscsi: Improve strings handling
17c3a52 scsi: target/iscsi: Make iscsit_ta_authentication() respect the output b
1edc254 x86/tsc: Add missing header to tsc_msr.c
4fc95d5 powerpc/kdump: Handle crashkernel memory reservation failure
084dad9 media: exynos4-is: Prevent NULL pointer dereference in __isp_video_try_f
ec9147b USB: serial: kobil_sct: fix modem-status error handling
81f7ce1 uwb: hwa-rc: fix memory leak at probe
9628ed4 x86/numa_emulation: Fix emulated-to-physical node mapping
64efd66 tsl2550: fix lux1_input error in low light
0d20b84 crypto: skcipher - Fix -Wstringop-truncation warnings
6b7066b HID: sony: Support DS4 dongle
88fc9f8 HID: sony: Update device ids
5e290d8 arm64: Add trace_hardirqs_off annotation in ret_to_user
17c3c6f ext4: don't mark mmp buffer head dirty
c77f7cc ext4: fix online resize's handling of a too-small final block group
4fdc69d ext4: recalucate superblock checksum after updating free blocks/inodes
83a2774 ext4: avoid divide by zero fault when deleting corrupted inline director
632ff8f ocfs2: fix ocfs2 read block panic
d31152b scsi: target: iscsi: Use hex2bin instead of a re-implementation
2e421bf ipv6: fix possible use-after-free in ip6_xmit()
3f0d9d1 neighbour: confirm neigh entries when ARP packet is received
a9b7eba net: hp100: fix always-true check for link up state
2ababd5 net/appletalk: fix minor pointer leak to userspace in SIOCFINDIPDDPRT
0aced03 gso_segment: Reset skb->mac_len after modifying network header
b457061 mm: shmem.c: Correctly annotate new inodes for lockdep
05bc6cb ring-buffer: Allow for rescheduling when removing pages
b27adc0 ALSA: emu10k1: fix possible info leak to userspace on SNDRV_EMU10K1_IOCT
7ddd41b ALSA: bebob: use address returned by kmalloc() instead of kernel stack f
b3667b7 ASoC: cs4265: fix MMTLR Data switch control
d1168b8 ANDROID: sdcardfs: Change current->fs under lock
cf59897 ANDROID: sdcardfs: Don't use OVERRIDE_CRED macro
9a8c091 PRIMA : Merge tag 'LA.UM.6.6.r1-09900-89xx.0' of https://source.codeauro
5170af1 Merge tag 'LA.UM.6.6.r1-09900-89xx.0' of https://source.codeaurora.org/q
b1b1ba1 asoc : msm: Fix zero size pointer issue
f3c4f38 Merge 1d019fd4b4649bbfddb00289b87ccbd6285b7d06 on remote branch
994d6e7 Merge 8a22a653e4730973bf26cd4415c74c8c7bb7224f on remote branch
336e264 drivers: mmc, usb: Pull missing 3.18.{20->71} changes
fead882 USB: u_ether: Squash some partial reverts
b5211f1 Revert "usb: dwc3: gadget: Fix calculation of request.actual for SG"
0c7771a Revert "usb: hcd: Fix double free with bandwidth_mutex on cable disconne

---
    ***********************************2018-10-01***********************************

---

*   336e264 drivers: mmc, usb: Pull missing 3.18.{20->71} changes
*   fead882 USB: u_ether: Squash some partial reverts
*   b5211f1 Revert "usb: dwc3: gadget: Fix calculation of request.actual for SG"
*   0c7771a Revert "usb: hcd: Fix double free with bandwidth_mutex on cable disconnect"
*   b4bb8e9 PRIMA : Merge tag 'LA.UM.6.6.r1-09800-89xx.0'
*   4be4ed7 Merge branch 'kernel.lnx.3.18.r33-rel' of https://github.com/android-linux-stable/msm-3.18 into v3.18y
*   301b720 Merge tag 'LA.UM.6.6.r1-09800-89xx.0' into kernel.lnx.3.18.r33-rel
*   65ad5e5 Renamed kernel zip to v3.18.123
*   66e69f9 Merge branch 'kernel.lnx.3.18.r33-rel' of https://github.com/android-linux-stable/msm-3.18 into v3.18y
*   ba3cc5b Merge 3.18.123 into kernel.lnx.3.18.r33-rel
*   921b2fe Linux 3.18.123
*   66688f6 USB: serial: ti_usb_3410_5052: fix array underflow in completion handler
*   cf9bbea drm/panel: type promotion bug in s6e8aa0_read_mtp_id()
*   32ab731 ALSA: pcm: Fix snd_interval_refine first/last with open min/max
*   4a8fd04 rtc: bq4802: add error handling for devm_ioremap
*   4d50d94 parport: sunbpp: fix error return code
*   03ace9d ARM: hisi: check of_iomap and fix missing of_node_put
*   073b26b ARM: hisi: handle of_iomap and fix missing of_node_put
*   ebb9196 MIPS: loongson64: cs5536: Fix PCI_OHCI_INT_REG reads
*   0bcaafb mtdchar: fix overflows in adjustment of `count`
*   2e866a2 audit: fix use-after-free in audit_add_watch
*   1a92b39 binfmt_elf: Respect error return from `regset->active'
*   34f39bd CIFS: fix wrapping bugs in num_entries()
*   cece187 cifs: prevent integer overflow in nxt_dir_entry()
*   6f3e0e8 usb: cdc-wdm: Fix a sleep-in-atomic-context bug in service_outstanding_interrupt()
*   a89c7b5 USB: yurex: Fix buffer over-read in yurex_write()
*   2fd95e9 usb: misc: uss720: Fix two sleep-in-atomic-context bugs
*   a9cdf4c USB: serial: io_ti: fix array underflow in completion handler
*   c601d90 usb: host: u132-hcd: Fix a sleep-in-atomic-context bug in u132_get_frame()
*   da7a5b5 usb: Avoid use-after-free by flushing endpoints early in usb_set_interface()
*   fbc3588 USB: Add quirk to support DJI CineSSD
*   1556715 usb: Don't die twice if PCI xhci host is not responding in resume
*   9ca1bf5 Tools: hv: Fix a bug in the key delete code
*   9778987 IB/ipoib: Avoid a race condition between start_xmit and cm_rep_handler
*   bd4971c xen/netfront: fix waiting for xenbus state change
*   36a9916 pstore: Fix incorrect persistent ram buffer mapping
*   e6858a9 RDMA/cma: Protect cma dev list with lock
*   31f0ff1 platform/x86: toshiba_acpi: Fix defined but not used build warnings
*   9cac5f3 s390/qeth: reset layer2 attribute on layer switch
*   1437dd3 s390/qeth: fix race in used-buffer accounting
*   67f5abb mac80211: restrict delayed tailroom needed decrement
*   98cc982 powerpc/powernv: opal_put_chars partial write fix
*   8eb6f3c perf powerpc: Fix callchain ip filtering
*   026d9d4 fbdev: Distinguish between interlaced and progressive modes
*   2a227c0 perf powerpc: Fix callchain ip filtering when return address is in a register
*   a4e5e18 fbdev/via: fix defined but not used warning
*   f697031 video: goldfishfb: fix memory leak on driver remove
*   bae63ef fbdev: omapfb: off by one in omapfb_register_client()
*   955a815 mtd/maps: fix solutionengine.c printk format warnings
*   40c8637 MIPS: ath79: fix system restart
*   3916385 gfs2: Special-case rindex for gfs2_grow
*   0d46dec xfrm: fix 'passing zero to ERR_PTR()' warning
*   b741bcf ALSA: usb-audio: Fix multiple definitions in AU0828_DEVICE() macro
*   4601c47 ALSA: msnd: Fix the default sample sizes
*   2b8f74c mm: get rid of vmacache_flush_all() entirely
*   a4508e0 netfilter: x_tables: avoid stack-out-of-bounds read in xt_copy_counters_from_user
*   449fab4 xhci: Fix use-after-free in xhci_free_virt_device
*   8456295 MIPS: WARN_ON invalid DMA cache maintenance, not BUG_ON
*   ae3ab8f f2fs: fix to do sanity check with {sit,nat}_ver_bitmap_bytesize
*   7092eb8 mfd: ti_am335x_tscadc: Fix struct clk memory leak
*   c919a68 partitions/aix: fix usage of uninitialized lv_info and lvname structures
*   845a0a1 partitions/aix: append null character to print data from disk
*   2541d77 net: dcb: For wild-card lookups, use priority -1, not 0
*   351bce3 net: mvneta: fix mtu change on port without link
*   d859640 gpio: ml-ioh: Fix buffer underwrite on probe error path
*   0492481 x86/mm: Remove in_nmi() warning from vmalloc_fault()
*   128b374 Bluetooth: hidp: Fix handling of strncpy for hid->name information
*   9e8f26c scsi: 3ware: fix return 0 on the error path of probe
*   a9ab273 ata: libahci: Correct setting of DEVSLP register
*   220146d MIPS: Fix ISA virt/bus conversion for non-zero PHYS_OFFSET
*   412d0c7 ath10k: prevent active scans on potential unusable channels
*   9e4dac3 macintosh/via-pmu: Add missing mmio accessors
*   4d9f6cf tty: rocket: Fix possible buffer overwrite on register_PCI
*   9b48a68 uio: potential double frees if __uio_register_device() fails
*   f2675e3 md/raid5: fix data corruption of replacements after originals dropped
*   cb8ef13 scsi: target: fix __transport_register_session locking
*   209c27b Bluetooth: h5: Fix missing dependency on BT_HCIUART_SERDEV
*   45845e2 staging/rts5208: Fix read overflow in memcpy
*   0ee00fd staging: rt5208: Fix a sleep-in-atomic bug in xd_copy_page
*   7ec6398 kthread: fix boot hang (regression) on MIPS/OpenRISC
*   3fb2459 kthread: Fix use-after-free if kthread fork fails
*   689d2103 cfq: Give a chance for arming slice idle timer in case of group_idle
*   933ce26 i2c: xiic: Make the start and the byte count write atomic
*   cb4009e ASoC: wm8994: Fix missing break in switch
*   dd6ff29 Fixes: Commit 86af955d02bb ("mm: numa: avoid waiting on freed migrated pages")
*   566f4e2 enic: do not call enic_change_mtu in enic_probe
*   f24049f irda: Only insert new objects into the global database via setsockopt
*   9f0547e irda: Fix memory leak caused by repeated binds of irda socket
*   2daf1a7 kbuild: make missing $DEPMOD a Warning instead of an Error
*   fa2d7df debugobjects: Make stack check warning more informative
*   174b32e btrfs: Don't remove block group that still has pinned down bytes
*   56f338b btrfs: relocation: Only remove reloc rb_trees if reloc control has been initialized
*   cb17dca btrfs: replace: Reset on-disk dev stats value after replace
*   5fcb40f powerpc/pseries: Avoid using the size greater than RTAS_ERROR_LOG_MAX.
*   5a16326 SMB3: Number of requests sent should be displayed for SMB3 not just CIFS
*   bf638d3 smb3: fix reset of bytes read and written stats
*   d4d5347 selftests/powerpc: Kill child processes on SIGINT
*   c2ff519 staging: comedi: ni_mio_common: fix subdevice flags for PFI subdevice
*   dc5b991 dm kcopyd: avoid softlockup in run_complete_job
*   801edd7 PCI: mvebu: Fix I/O space end address calculation
*   bd724a4 scsi: aic94xx: fix an error code in aic94xx_init()
*   4d94096 s390/dasd: fix hanging offline processing due to canceled worker
*   f0d26e4 powerpc: Fix size calculation using resource_size()
*   47e5fde net/9p: fix error path of p9_virtio_probe
*   022e1fb platform/x86: asus-nb-wmi: Add keymap entry for lid flip action on UX360
*   d03b202 mfd: sm501: Set coherent_dma_mask when creating subdevices
*   4b351b9 ipvs: fix race between ip_vs_conn_new() and ip_vs_del_dest()
*   06d14c2 mm/fadvise.c: fix signed overflow UBSAN complaint
*   dd36e88 scripts: modpost: check memory allocation results
*   35eb26e fat: validate ->i_start before using
*   c0aa362 reiserfs: change j_timestamp type to time64_t
*   5d1346a fork: don't copy inconsistent signal handler state to child
*   5bbef60 hfs: prevent crash on exit from failed search
*   8224be0 hfsplus: don't return 0 when fill_super() failed
*   0b7ebfb cifs: check if SMB2 PDU size has been padded and suppress the warning

---
    ***********************************2018-09-11***********************************

---

*   8118380 (PRIMA) Merge tag 'LA.UM.6.6.r1-09700-89xx.0'
*   39e971d Merge branch 'kernel.lnx.3.18.r33-rel' of https://github.com/android-linux-stable/msm-3.18 into v3.18y
*   a5cf0ab Merge tag 'LA.UM.6.6.r1-09700-89xx.0' into kernel.lnx.3.18.r33-rel
*   a286f86 Renamed kernel zip to v3.18.122
*   1400bd6 sched/core: Properly fix constant logical operand Clang warning
*   560a6bd fix memory leak free binder memory on error
*   958bb18 disable mdss xlog panic on error
*   e537088 msm: ipa3: Fix redundant wakelock releases in error paths
*   e737632 Merge branch 'kernel.lnx.3.18.r33-rel' of https://github.com/android-linux-stable/msm-3.18 into caf
*   09f1173 Merge 3.18.122 into kernel.lnx.3.18.r33-rel
*   c030599 Linux 3.18.122
*   b271f88 bcache: release dc->writeback_lock properly in bch_writeback_thread()
*   054206a getxattr: use correct xattr length
*   6f2f65e udlfb: set optimal write delay
*   7639111 fb: fix lost console when the user unplugs a USB adapter
*   6c4dcc2 pwm: tiehrpwm: Fix disabling of output of PWMs
*   37ca931 ubifs: Fix synced_i_size calculation for xattr inodes
*   d651012 Revert "UBIFS: Fix potential integer overflow in allocation"
*   155279d ubifs: Fix memory leak in lprobs self-check
*   7d024b6 userns: move user access out of the mutex
*   8a749f3 userns; Correct the comment in map_write
*   a1ca395 sys: don't hold uts_sem while accessing userspace memory
*   3680c7e osf_getdomainname(): use copy_to_user()
*   76b5c9f mm/tlb: Remove tlb_remove_table() non-concurrent condition
*   8c6a5c9 ARM: tegra: Fix Tegra30 Cardhu PCA954x reset
*   86e40c0 pnfs/blocklayout: off by one in bl_map_stripe()
*   02de522 9p: fix multiple NULL-pointer-dereferences
*   eb67901 uprobes: Use synchronize_rcu() not synchronize_sched()
*   73b5c3d kthread, tracing: Don't expose half-written comm when creating kthreads
*   a5a4dfa tracing/blktrace: Fix to allow setting same value
*   38a39e3 tracing: Do not call start/stop() functions when tracing_on does not change
*   76eb62b iio: ad9523: Fix return value for ad952x_store()
*   a3442d6 iio: ad9523: Fix displayed phase
*   ceef7b2 dm cache metadata: save in-core policy_hint_size to on-disk superblock
*   d90fb29 net/9p/trans_fd.c: fix race-condition by flushing workqueue before the kfree()
*   7bba0ec net/9p/client.c: version pointer uninitialized
*   fd38cf6 9p/virtio: fix off-by-one error in sg list bounds check
*   43a2089 powerpc/pseries: Fix endianness while restoring of r3 in MCE handler.
*   b3f3454 powerpc/fadump: handle crash memory ranges array index overflow
*   fec7d72 spi: davinci: fix a NULL pointer dereference
*   569bded ALSA: rawmidi: Undo my 3.18.117 resolution

