- git clone git@github.com:lhvu2/bwa-mem2.git
- cd bwa-mem2
- git submodule init
- git submodule update
make
- export $PATH=`pwd`:$PATH (to set bwa-mem2 in the $PATH)
- source ~/.bashrc


1. cd /home/lhvu/bio/bioinfo-notebook/tests/ex6-bwa-mem2/reference
2. bwa-mem2 index lambda_virus.fa
4. Output:

```
(base) lhvu@optus0622:~/bio/bwa-mem2$ cd ../bioinfo-notebook/tests/ex6-bwa-mem2/
(base) lhvu@optus0622:~/bio/bioinfo-notebook/tests/ex6-bwa-mem2$ cd reference/
(base) lhvu@optus0622:~/bio/bioinfo-notebook/tests/ex6-bwa-mem2/reference$ bwa-mem2 index lambda_virus.fa
Looking to launch executable "/home/lhvu/bio/bwa-mem2/bwa-mem2.avx2", simd = .avx2
Launching executable "/home/lhvu/bio/bwa-mem2/bwa-mem2.avx2"
[bwa_index] Pack FASTA... 0.00 sec
* Entering FMI_search
init ticks = 3366798
ref seq len = 97004
binary seq ticks = 2305914
build suffix-array ticks = 15120096
ref_seq_len = 97004
count = 0, 24320, 48502, 72684, 97004
BWT[65380] = 4
CP_SHIFT = 6, CP_MASK = 63
sizeof CP_OCC = 64
pos: 12126, ref_seq_len__: 12125
max_occ_ind = 1515
build fm-index ticks = 4873616
Total time taken: 0.0138
```
