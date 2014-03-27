Variant Calling BWA Workflow
============================

A variant calling workflow based on the BWA read mapper and the mpileup variant caller.

Description
-----------

This workflow detects small variations like SNPs or indels that occur in a paired-end sequenced sample genome in comparison to a reference genome. The input is a reference genome given in Fasta format and two read files of *left* and *right* ends (can be interchanged) of the sequenced paired-end reads in Fasta or Fastq format. Output is a text file in VCF format whose lines contain the detected variants.

The workflow consists of a read mapping step where BWA is used to index the genome and map reads onto it. The aligned reads are then converted from SAM to BAM format and sorted by genome position. In the second step the read alignments are transposed into the pileup format which for each genomic position stores the read bases that are aligned to it. From the set of bases deviating from the reference genome, mpileup calls variants and outputs them in BCF format which is finally converted in the human-readable VCF format.

![alt tag](variant_calling_bwa_screenshot.png)


Example Data
------------

Configure the three *Input File* nodes accordingly:

<dl>
  <dt>INPUT Reference</dt>
  <dd>NC_008253_1K.fa - First 1kb of the E.coli genome.</dd>

  <dt>INPUT Left Reads</dt>
  <dd>sim_reads_l.fq - Left reads of 10k paired-end reads of a simulated haplotype.</dd>
  
  <dt>INPUT Right Reads</dt>
  <dd>sim_reads_r.fq - Right reads of 10k paired-end reads of a simulated haplotype.</dd>
</dl>  


References
----------

**BWA Website:**
  http://bio-bwa.sourceforge.net

**mpileup Website:**
  http://samtools.sourceforge.net/mpileup.shtml

