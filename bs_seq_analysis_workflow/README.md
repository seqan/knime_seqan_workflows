BS-Seq Workflow
===============

todo

Description
-----------

todo

![alt tag](bs_seq_analysis_workflow.png)

Prerequisites
-------------

Make sure that the following prerequisites are installed:
- SeqAn NGS ToolBox (see [installation instructions](http://trac.seqan.de/wiki/HowTo/UseSeqAnNodesInKnime#InstallSeqAninKNIME))

Example Data
------------

Extract the example_data.zip file and configure the three *Input File* nodes accordingly:

<dl>
  <dt>Genome</dt>
  <dd><ul>
  <li>hg18_chr21_micro.fa</li>
  </ul>
  Small sequence of 300kb sampled from human chr21.</dd>
  <dt>Left and Right Reads</dt>
  <dd><ul>
  <li>reads_pe_N48000.L.fastq.fa</li>
  <li>reads_pe_N48000.R.fastq.fa</li>
  </ul>
  Simulated reads from methylated haplotypes.</dd>
</dl>  

Output
------

todo

References
----------

Sabrina Krakau. *Developing a BS-Seq Analysis Workflow for Genomic Variation and Methylation Level Calling*, [MSc Thesis](http://www.mi.fu-berlin.de/en/inf/groups/abi/theses/master_dipl/krakau/msc_thesis_krakau.pdf)
