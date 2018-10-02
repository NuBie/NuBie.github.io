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

