1. cd /home/lhvu/bio/bioinfo-notebook/tests/ex2-bowtie2
2. export BOWTIE2_INDEXES=`pwd`/index
3. bowtie2 --no-unal -p 8 -x lambda_virus  -1 reads/reads_1.fq -2 reads/reads_2.fq -S output_bowtie2.sam
4. Output:

```
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex2$ bowtie2 --no-unal -p 8 -x lambda_virus  -1 reads/reads_1.fq -2 reads/reads_2.fq -S output.sam
10000 reads; of these:
  10000 (100.00%) were paired; of these:
    834 (8.34%) aligned concordantly 0 times
    9166 (91.66%) aligned concordantly exactly 1 time
    0 (0.00%) aligned concordantly >1 times
    ----
    834 pairs aligned concordantly 0 times; of these:
      42 (5.04%) aligned discordantly 1 time
    ----
    792 pairs aligned 0 times concordantly or discordantly; of these:
      1584 mates make up the pairs; of these:
        1005 (63.45%) aligned 0 times
        579 (36.55%) aligned exactly 1 time
        0 (0.00%) aligned >1 times
94.97% overall alignment rate
```
