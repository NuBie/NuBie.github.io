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



---
    ***********************************2018-09-08***********************************

---

*   ef8e4bd Renamed kernel zip to v3.18.121
*   f92fc22 workqueue: fix permissions for power-efficient_wq
*   6f055a6 UPSTREAM: fs/sync.c: remove unnecessary NULL f_mapping check in sync_fil
*   2c827d1 USB: f_fs: change wait as freezable
*   663b176 cpufreq: Restore policy min/max limits on CPU online
*   18fd313 arm64: Use optimized memcmp
*   bbfc548 cpufreq: conservative: unlock sample_rate
*   f3b2058 cpufreq: conservative: Decrease frequency faster when the timer deferred
*   8a95b50 msm: mdss: update mdss perf when changing refresh rate
*   0994c81 prevent false check on qcom cpufreq
*   42ab924 Add USB HID gadget suport
*   0adaa46 Makefile: fix segfaults when compiled with Clang
*   aca5ce2 Revert "sched: qhmp: avoid scheduling RT threads on cores currently hand
*   7c3d3f7 msm: kgsl: Remove POPP
*   0604113 Merge remote-tracking branch 'als/kernel.lnx.3.18.r33-rel' into caf
*   8167c01 Merge 3.18.121 into kernel.lnx.3.18.r33-rel
*   ba6984f Linux 3.18.121
*   2f29438 cdrom: Fix info leak/OOB read in cdrom_ioctl_drive_status
*   86c0a64 scsi: core: Avoid that SCSI device removal through sysfs triggers a dead
*   a6abc93 scsi: sysfs: Introduce sysfs_{un,}break_active_protection()
*   1d7acd2 MIPS: Correct the 64-bit DSP accumulator register size
*   7ab91fb kprobes: Make list and blacklist root user read only
*   be4f8c4 s390/pci: fix out of bounds access during irq setup
*   dc826c9 s390/qdio: reset old sbal_state flags
*   0fd1986 pinctrl: freescale: off by one in imx1_pinconf_group_dbg_show()
*   3aeaed1 ASoC: sirf: Fix potential NULL pointer dereference
*   aa6ba5e udl-kms: fix crash due to uninitialized memory
*   953d8af udl-kms: handle allocation failure
*   8f02d4b udl-kms: change down_interruptible to down
*   e0dd67c fuse: Add missed unlock_page() to fuse_readpages_fill()
*   9b39c90 fuse: Don't access pipe->buffers without pipe_lock()
*   91196d9 x86/process: Re-export start_thread()
*   a030af4 KVM: arm/arm64: Skip updating PMD entry if no change
*   107c387 KVM: arm/arm64: Skip updating PTE entry if no change
*   872f590 arm64: mm: check for upper PAGE_SHIFT bits in pfn_valid()
*   1f9e541 ext4: reset error code in ext4_find_entry in fallback
*   ef2d2e2 s390/kvm: fix deadlock when killed by oom
*   8e46b77 btrfs: don't leak ret from do_chunk_alloc
*   4c41a07 mm/memory.c: check return value of ioremap_prot
*   f3ab050 scsi: vmw_pvscsi: Return DID_RESET for status SAM_STAT_COMMAND_TERMINATE
*   ea0f604 scsi: fcoe: drop frames in ELS LOGO error path
*   7ae3f84 drivers: net: lmc: fix case value for target abort error
*   0171efb arc: fix type warnings in arc/mm/cache.c
*   04b68e4 arc: fix build errors in arc/include/asm/delay.h
*   e5b4032 enic: handle mtu change for vf properly
*   af47ed8 Revert "MIPS: BCM47XX: Enable 74K Core ExternalSync for PCIe erratum"
*   417ea43 tools/power turbostat: Read extended processor family from CPUID
*   33a11da zswap: re-check zswap_is_full() after do zswap_shrink()
*   fdb2cd0 selftests/ftrace: Add snapshot and tracing_on test case
*   582db66 cachefiles: Wait rather than BUG'ing on "Unexpected object collision"
*   4eabf1e cachefiles: Fix refcounting bug in backing-file read monitoring
*   a60d078 fscache: Allow cancelled operations to be enqueued
*   903d5b8 net: axienet: Fix double deregister of mdio
*   73b89b6 bnx2x: Fix invalid memory access in rss hash config path.
*   da1ab9d media: staging: omap4iss: Include asm/cacheflush.h after generic include
*   b725b8a can: mpc5xxx_can: check of_iomap return before use
*   4dafaff atl1c: reserve min skb headroom
*   4794000 net: caif: Add a missing rcu_read_unlock() in caif_flow_cb
*   944dbf3 tools/power turbostat: fix -S on UP systems
*   2b8e010 usb: gadget: f_uac2: fix endianness of 'struct cntrl_*_lay3'
*   5461575 tools: usb: ffs-test: Fix build on big endian systems
*   a438b32 usb/phy: fix PPC64 build errors in phy-fsl-usb.c
*   97f07e5 usb: gadget: r8a66597: Fix a possible sleep-in-atomic-context bugs in r8
*   c51c58d usb: gadget: r8a66597: Fix two possible sleep-in-atomic-context bugs in 
*   2d72c0a drm/imx: imx-ldb: check if channel is enabled before printing warning
*   ce7c57f drm/imx: imx-ldb: disable LDB on driver bind
*   ad020ae scsi: libiscsi: fix possible NULL pointer dereference in case of TMF
*   115b738 nl80211: Add a missing break in parse_station_flags
*   491e335 mac80211: add stations tied to AP_VLANs during hw reconfig
*   0b389a6 xfrm: free skb if nlsk pointer is NULL
*   ea0926c xfrm: fix missing dst_release() after policy blocking lbcast and multica
*   9a21340 Cipso: cipso_v4_optptr enter infinite loop
*   319bc6c sched/sysctl: Check user input value of sysctl_sched_time_avg

