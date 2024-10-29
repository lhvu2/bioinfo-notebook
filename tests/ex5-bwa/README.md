- git clone git@github.com:lhvu2/bwa.git
- cd bwa
- make (this will install bwa binary)
- export $PATH=`pwd`:$PATH (to set bwa in the $PATH)
- source ~/.bashrc


1. cd /home/lhvu/bio/bioinfo-notebook/tests/ex5-bwa/reference
2. bwa index lambda_virus.fa
4. Output:

```
(base) lhvu@optus0622:~/bio/bioinfo-notebook/tests/ex5-bwa/reference$ bwa index lambda_virus.fa
[bwa_index] Pack FASTA... 0.00 sec
[bwa_index] Construct BWT for the packed sequence...
[bwa_index] 0.01 seconds elapse.
[bwa_index] Update BWT... 0.00 sec
[bwa_index] Pack forward-only FASTA... 0.00 sec
[bwa_index] Construct SA from BWT and Occ... 0.00 sec
[main] Version: 0.7.18-r1243-dirty
[main] CMD: bwa index lambda_virus.fa
[main] Real time: 0.020 sec; CPU: 0.018 sec
```
