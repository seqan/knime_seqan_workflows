Variant Calling BWA Workflow
============================

A variant calling workflow based on the BWA read mapper and the mpileup variant caller.

Description
-----------

coming soon

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

