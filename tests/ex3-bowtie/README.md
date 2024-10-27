1. cd /home/lhvu/bio/bioinfo-notebook/tests/ex3-bowtie
2. export BOWTIE_INDEXES=`pwd`/index
3. bowtie --no-unal -p 8 -x lambda_virus  -1 reads/reads_1.fq -2 reads/reads_2.fq -S output_bowtie.sam
4. Output:

```
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex3-bowtie$ bowtie --no-unal -p 8 -x lambda_virus  -1 reads/reads_1.fq -2 reads/reads_2.fq -S output_bowtie.sam
# reads processed: 10000
# reads with at least one alignment: 2157 (21.57%)
# reads that failed to align: 7843 (78.43%)
Reported 2157 paired-end alignments
```
