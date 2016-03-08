# ceph_kernel_module_backports
Backport ceph kernel modules from higher kernel version to 3.10.x

Directory Introduction
----------------------

kernel_src directory contains the relative path of ceph kernel modules source files against original 3.10.x kernel source tree.

ChangeLog
---------

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
  
