---
layout: post
title:  Oreo kernel for mido 
date:   2018-09-01 00:55:00 +0700
categories: guzzo tips
---
Ini adalah changelog perubahan Kernel mido v3.18.y based on caf untuk Android Oreo Treble yang telah di merged ke github repository ! sources dapat dilihat [Disini!](https://github.com/NuBie/android_kernel_xiaomi_msm8953)

Changelog/Tracking :
---
*   --common kernel--
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


---
    ***********************************2018-09-01***********************************

---

*   e3eabd9 Renamed kernel zip to v3.18.120
*   fc2f603 Merge remote-tracking branch 'als/kernel.lnx.3.18.r33-rel' into v3.18y
*   d35538e Merge 3.18.120 into kernel.lnx.3.18.r33-rel
*   a5f9be3 Linux 3.18.120
*   88f8dcd reiserfs: fix broken xattr handling (heap corruption, bad retval)
*   3311a39 PCI: hotplug: Don't leak pci_slot on registration failure
*   c1d01e1 packet: refine ring v3 block size test to hold one frame
*   c022960 netfilter: conntrack: dccp: treat SYNC/SYNCACK as invalid if no prior state
*   966e597 xfrm_user: prevent leaking 2 bytes of kernel memory
*   5554e8f staging: android: ion: check for kref overflow
*   dfd3805 tcp: identify cryptic messages as TCP seq # bugs
*   45d5a5d net: qca_spi: Make sure the QCA7000 reset is triggered
*   1357eab net: qca_spi: Avoid packet drop during initial sync
*   01c755b net: usb: rtl8150: demote allmulti message to dev_dbg()
*   9012fe0 qlogic: check kstrtoul() for errors
*   89a9bc2 ixgbe: Be more careful when modifying MAC filters
*   c76800b ARM: dts: am3517.dtsi: Disable reference to OMAP3 OTG controller
*   7fed6b5 drm/armada: fix colorkey mode property
*   f8ebc47 ARM: pxa: irq: fix handling of ICMR registers in suspend/resume
*   2e792ad netfilter: x_tables: set module owner for icmp(6) matches
*   46ed892 smsc75xx: Add workaround for gigabit link up hardware errata.
*   766c02b tracing: Use __printf markup to silence compiler
*   d982378 ARM: imx_v4_v5_defconfig: Select ULPI support
*   d35f874 m68k: fix "bad page state" oops on ColdFire boot
*   7af7d6ec bnx2x: Fix receiving tx-timeout in error or recovery state.
*   f4ed9d9 drm/exynos: gsc: Fix support for NV16/61, YUV420/YVU420 and YUV422 modes
*   0d8e0d1 md/raid10: fix that replacement cannot complete recovery after reassemble
*   c641c71 dmaengine: k3dma: Off by one in k3_of_dma_simple_xlate()
*   a750989 ARM: dts: da850: Fix interrups property for gpio
*   915d80f perf report powerpc: Fix crash if callchain is empty
*   9b99d54 ARM: dts: am437x: make edt-ft5x06 a wakeup source
*   7acdfae brcmfmac: stop watchdog before detach and free everything
*   99b61ce cxgb4: when disabling dcb set txq dcb priority to 0
*   f1630f8 Smack: Mark inode instant in smack_task_to_inode
*   79093b9 ipv6: mcast: fix unsolicited report interval after receiving querys
*   9773c6d locking/lockdep: Do not record IRQ state within lockdep code
*   a5eb5cb net: davinci_emac: match the mdio device against its compatible if possible
*   d4a1dd4 net: propagate dev_get_valid_name return code
*   318b0e8 net: hamradio: use eth_broadcast_addr
*   2416eb0 enic: initialize enic->rfs_h.lock in enic_probe
*   f26b61f arm64: make secondary_start_kernel() notrace
*   c302a0e usb: gadget: composite: fix delayed_status race condition when set_interface
*   bd3db43 usb: dwc2: fix isoc split in transfer with no data
*   3b0134e selftests: sync: add config fragment for testing sync framework
*   20b50fb netfilter: ipv6: nf_defrag: reduce struct net memory waste
*   f6d57da isdn: Disable IIOCDBGVAR
*   9515219 Bluetooth: avoid killing an already killed socket
*   0af583b serial: 8250_dw: always set baud rate in dw8250_set_termios
*   382627a USB: serial: sierra: fix potential deadlock at close
*   23a5e85 ALSA: vxpocket: Fix invalid endian conversions
*   270ba2c ALSA: memalloc: Don't exceed over the requested size
*   88c9ef7 ALSA: cs5535audio: Fix invalid endian conversion
*   75890e9 ALSA: virmidi: Fix too long output trigger loop
*   9c09519 ALSA: vx222: Fix invalid endian conversions
*   2ccea62 vsock: split dwork to avoid reinitializations
*   31b912a5 net_sched: fix NULL pointer dereference when delete tcindex filter
*   8a6eecd net_sched: Fix missing res info when create new tc_index filter
*   71e6f3f llc: use refcount_inc_not_zero() for llc_sap_find()
*   719710e l2tp: use sk_dst_check() to avoid race on sk->sk_dst_cache
*   63615fa dccp: fix undefined behavior with 'cwnd' shift in ccid2_cwnd_restart()
