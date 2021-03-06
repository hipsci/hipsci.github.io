---
layout: page
title: RNA sequencing
permalink: /assay/rnaseq/
---

RNA sequencing is performed on all HipSci iPS cell lines that are selected for banking
after passing QC. Sequencing and primary analysis are performed at the
Wellcome Trust Sanger Institue.

###Primary analysis

HipSci's RNA-seq analysis pipeline is to 
map sequence reads to the human GRCh37 reference using the
[STAR spliced aligner](https://github.com/alexdobin/STAR). The mapping uses
version 19 of the Gencode gene annotation to enable splice-aware alignments.


###Getting the data

Complete lists of exome-seq data can be found under the files tab of
the [cell lines and data browser]({{'/lines/#/files?Assay[]=RNA-seq' | prepend: site.baseurl}})
or in the dataset indexes on the [FTP site](ftp://ftp.hipsci.ebi.ac.uk/vol1/ftp/archive_datasets/).

* [Raw sequencing reads]({{'/lines/#/files?Assay[]=RNA-seq&Description[]=Raw%20sequencing%20reads' | prepend: site.baseurl }})
-- Distributed in the cram file format. Any cell line
can have multiple associated cram files; each corresponds to a single lane of sequencing.
* [Splice-aware STAR alignment]({{'/lines/#/files?Assay[]=Exome-seq&Description[]=Splice-aware%20STAR%20alignment' | prepend: site.baseurl }})
-- Distributed in the bam file format.  We distribute one bam file per cell line.

For [managed access](/data/faq/find-download-managed-access-files) cell lines, RNA-seq
files are archived in the [EGA](https://ega-archive.org/). The
[data browser]({{'/lines/#/files?Assay[]=RNA-seq' | prepend: site.baseurl}}) contains
links to the relevant EGA dataset page, from where researchers can request access to the data.

For [open access](/data/faq/find-download-open-access-files) cell lines, RNA-seq files
are archived in [ENA](http://www.ebi.ac.uk/ena/data/view/ERP007111). Data are openly available
to anybody, and the [data browser]({{'/lines/#/files?Assay[]=RNA-seq' | prepend: site.baseurl}})
contains direct links to the files on the ENA FTP server.


###Resources

HipSci's FTP site contains:

* The [reference genome](ftp://ftp.hipsci.ebi.ac.uk/vol1/ftp/reference/) used for alignment
* The [Gencode gene annotations](ftp://ftp.hipsci.ebi.ac.uk/vol1/ftp/reference/) used for splice-aware
alignment.
