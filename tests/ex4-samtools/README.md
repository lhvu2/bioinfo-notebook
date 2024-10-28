```
Follow the instructions here to install samtools and bcftools.
https://www.htslib.org/download/

cd samtools-1.x    # and similarly for bcftools and htslib
./configure --prefix=/where/to/install
make
make install

samtools in: /home/lhvu/bio/samtools-1.21/bin, bcftools in /home/lhvu/bio/bcftools-1.21/bin.

Add these two folders into the $PATH env
```

Using samtools
```
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex4-samtools$ pwd
/home/lhvu/bio/bioinfo-notebook/tests/ex4-samtools
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex4-samtools$ ls ../ex2-bowtie2/
index  output_bowtie2.sam  README.md  reads  reference
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex4-samtools$ samtools view -@ n -Sb -o example_alignment.bam ../ex2-bowtie2/output_bowtie2.sam
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex4-samtools$ ls
example_alignment.bam  README.md
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex4-samtools$ file example_alignment.bam
example_alignment.bam: Blocked GNU Zip Format (BGZF; gzip compatible), block length 329
(base) lhvu@realtimeaidoe:~/bio/bioinfo-notebook/tests/ex4-samtools$

```