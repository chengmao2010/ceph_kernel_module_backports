# ceph_kernel_module_backports
Backport ceph kernel modules from higher kernel version to 3.10.x

Directory Introduction
----------------------

kernel_src directory contains the relative path of ceph kernel modules source files against original 3.10.x kernel source tree.

ChangeLog
---------

* [2016-3-11]
  * Backport some cephfs critical fixes from 4.5 to 3.10.94 (some of them may be modified a little on 3.10.94)
    * https://git.kernel.org/cgit/linux/kernel/git/stable/linux-stable.git/commit/fs/ceph?id=979abfdd5c7ca4abe3f0157a6ea9bfef41114c89
    * https://git.kernel.org/cgit/linux/kernel/git/stable/linux-stable.git/commit/fs/ceph?id=a096b09aeec6ff99edfdfd8cee24d6f25377d585
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/fs/ceph/file.c?h=v4.5-rc7&id=ab866549b3da3eef88e51696bcb24e79f1cc3745
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/fs/ceph?h=v4.5-rc7&id=a56371d9d920799ebb88c196aa018e76fc46554f
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/?id=5e804ac4824302efc3038e086cb21f2e93ab8900
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/fs/ceph?h=v4.5-rc7&id=687265e5a885d6308f5d73e738efe3c2674fa218
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/fs/ceph?h=v4.5-rc7&id=a149bb9a281c5c2904cf6fcdf9ed386340032ce3
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/fs/ceph?h=v4.5-rc7&id=0081bd83c089ef3d0c9a4e4e869e2ab75f2cb379
    * https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/commit/fs/ceph?h=v4.5-rc7&id=a30be7cb2ccb995ad5e67fd4b548f11fe37fc8b1

* [2016-3-1]:
  * Backport cache tier support on kernel cephfs from 3.18.20 to 3.10.94
    * https://git.kernel.org/cgit/linux/kernel/git/stable/linux-stable.git/commit/include/linux/ceph/ceph_features.h?id=80e163a58c0c69ef1a0ba3500d9932b14d67bf64
    * http://www.spinics.net/lists/ceph-devel/msg17436.html

* [2015-12-25]:
  * Initial backport from kernel 3.18.20 to 3.10.90 for cephfs module

* [2015-9-8]:
  * Backport tcp_nodelay support from kernel 4.2 to 3.10.83
    * https://git.kernel.org/cgit/linux/kernel/git/stable/linux-stable.git/commit/include/linux/ceph?id=ba988f87f532cd2b8c4740aa8ec49056521ae833
    * https://git.kernel.org/cgit/linux/kernel/git/stable/linux-stable.git/commit/net/ceph?id=ba988f87f532cd2b8c4740aa8ec49056521ae833

* [2015-9-2]:
  * Initial backport from kernel 3.18.20 to 3.10.83 for rbd and libceph modules
  
