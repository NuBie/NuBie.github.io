---
layout: post
title:  Oreo kernel for mido 
date:   2018-09-01 00:55:00 +0700
categories: guzzo tips
---
Ini adalah Kernel based on caf dari mido untuk oreo treble 

---
Changelog :

e3eabd9 Renamed kernel zip to v3.18.120
fc2f603 Merge remote-tracking branch 'als/kernel.lnx.3.18.r33-rel' into v3.18y
d35538e Merge 3.18.120 into kernel.lnx.3.18.r33-rel
a5f9be3 Linux 3.18.120
88f8dcd reiserfs: fix broken xattr handling (heap corruption, bad retval)
3311a39 PCI: hotplug: Don't leak pci_slot on registration failure
c1d01e1 packet: refine ring v3 block size test to hold one frame
c022960 netfilter: conntrack: dccp: treat SYNC/SYNCACK as invalid if no prior state
966e597 xfrm_user: prevent leaking 2 bytes of kernel memory
5554e8f staging: android: ion: check for kref overflow
dfd3805 tcp: identify cryptic messages as TCP seq # bugs
45d5a5d net: qca_spi: Make sure the QCA7000 reset is triggered
1357eab net: qca_spi: Avoid packet drop during initial sync
01c755b net: usb: rtl8150: demote allmulti message to dev_dbg()
9012fe0 qlogic: check kstrtoul() for errors
89a9bc2 ixgbe: Be more careful when modifying MAC filters
c76800b ARM: dts: am3517.dtsi: Disable reference to OMAP3 OTG controller
7fed6b5 drm/armada: fix colorkey mode property
f8ebc47 ARM: pxa: irq: fix handling of ICMR registers in suspend/resume
2e792ad netfilter: x_tables: set module owner for icmp(6) matches
46ed892 smsc75xx: Add workaround for gigabit link up hardware errata.
766c02b tracing: Use __printf markup to silence compiler
d982378 ARM: imx_v4_v5_defconfig: Select ULPI support
d35f874 m68k: fix "bad page state" oops on ColdFire boot
7af7d6ec bnx2x: Fix receiving tx-timeout in error or recovery state.
f4ed9d9 drm/exynos: gsc: Fix support for NV16/61, YUV420/YVU420 and YUV422 modes
0d8e0d1 md/raid10: fix that replacement cannot complete recovery after reassemble
c641c71 dmaengine: k3dma: Off by one in k3_of_dma_simple_xlate()
a750989 ARM: dts: da850: Fix interrups property for gpio
915d80f perf report powerpc: Fix crash if callchain is empty
9b99d54 ARM: dts: am437x: make edt-ft5x06 a wakeup source
7acdfae brcmfmac: stop watchdog before detach and free everything
99b61ce cxgb4: when disabling dcb set txq dcb priority to 0
f1630f8 Smack: Mark inode instant in smack_task_to_inode
79093b9 ipv6: mcast: fix unsolicited report interval after receiving querys
9773c6d locking/lockdep: Do not record IRQ state within lockdep code
a5eb5cb net: davinci_emac: match the mdio device against its compatible if possible
d4a1dd4 net: propagate dev_get_valid_name return code
318b0e8 net: hamradio: use eth_broadcast_addr
2416eb0 enic: initialize enic->rfs_h.lock in enic_probe
f26b61f arm64: make secondary_start_kernel() notrace
c302a0e usb: gadget: composite: fix delayed_status race condition when set_interface
bd3db43 usb: dwc2: fix isoc split in transfer with no data
3b0134e selftests: sync: add config fragment for testing sync framework
20b50fb netfilter: ipv6: nf_defrag: reduce struct net memory waste
f6d57da isdn: Disable IIOCDBGVAR
9515219 Bluetooth: avoid killing an already killed socket
0af583b serial: 8250_dw: always set baud rate in dw8250_set_termios
382627a USB: serial: sierra: fix potential deadlock at close
23a5e85 ALSA: vxpocket: Fix invalid endian conversions
270ba2c ALSA: memalloc: Don't exceed over the requested size
88c9ef7 ALSA: cs5535audio: Fix invalid endian conversion
75890e9 ALSA: virmidi: Fix too long output trigger loop
9c09519 ALSA: vx222: Fix invalid endian conversions
2ccea62 vsock: split dwork to avoid reinitializations
31b912a5 net_sched: fix NULL pointer dereference when delete tcindex filter
8a6eecd net_sched: Fix missing res info when create new tc_index filter
71e6f3f llc: use refcount_inc_not_zero() for llc_sap_find()
719710e l2tp: use sk_dst_check() to avoid race on sk->sk_dst_cache
63615fa dccp: fix undefined behavior with 'cwnd' shift in ccid2_cwnd_restart()
