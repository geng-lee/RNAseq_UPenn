# Overview

In this class we’ll discuss how you can use R/Bioconductor to tap into vast amounts of RNAseq data available through the Sequence Read Archive (SRA) and Gene Expression Omnibus (GEO).

## Learning objectives

* Learn about fasterq_dump
* Learn about HDF5 file format
* Explore ARCHS4 database programatically
* Start and finish the Step 4 script

## Downloads

ARCHS4 database in HDF5 format for [human](https://www.dropbox.com/s/t9umqxu5ahsy9rc/human_matrix_v8.h5?dl=0) and [mouse](https://www.dropbox.com/s/crz1ctpqhbpb1ox/mouse_matrix_v8.h5?dl=0). These HDF5 files contain RNAseq data already aligned using Kallisto for 238,522 and 284,907 samples, respectively. Note that each of these files will take about ~7GB of space on your hard-drive. For the purposes of this lecture, you only need to download the mouse data.

## Reading

* [Massive mining of publicly available RNA-seq data from human and mouse. Nature Communications, April, 2018](https://www.nature.com/articles/s41467-018-03751-6). Describes the ARCHS4 resource from Avi Ma’ayan’s lab that provides convenient access to public RNAseq datasets, already prealigned with Kallisto. You can access data either through the [ARCHS4 website](https://amp.pharm.mssm.edu/archs4/) or using the [rhdf5 package](https://www.bioconductor.org/packages/devel/bioc/vignettes/rhdf5/inst/doc/rhdf5.html).
* [Digital Expression Explorer 2: a repository of 4.5 trillion uniformly processed RNA-seq reads and counting](https://zenodo.org/record/1561840#.XIlI0hNKjOQ) - similar to ARCHS4, the DEE2 project leverages Kallisto and GEO/SRA to make hundreds of thousands of samples readily available to you, either through [their website](http://dee2.io/), or through R using the [DEE2 package](https://github.com/markziemann/dee2/blob/master/AccessDEEfromR.md).
* [Activity of Uncleaved Caspase-8 Controls Anti-bacterial Immune Defense and TLR-Induced Cytokine Production Independent of Cell Death, Oct, 2016](https://journals.plos.org/plospathogens/article?id=10.1371/journal.ppat.1005910). This paper contains the data we’ll retrieve from a public gene expression repository. The data is available [here](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE86922).

### Other video

[ARCHS4 video](https://youtu.be/TjkWSBQuKoE) describing how HDF5 files were created from gene expression data (13 min)
