# RiVIERA-MT
<u>Ri</u>sk <u>V</u>ariant <u>I</u>nference using <u>E</u>pigenomic <u>R</u>eference <u>A</u>nnotation to predict <u>M</u>ultiple <u>T</u>rait-causing co-localized mutations

## Description
RiVIERA-MT is a full Bayesian framework to fine-map causal variants using GWAS summary statistics in z-scores in one or multiple related traits and large-scale reference annotations in binary or continuous values. The goal of RiVIERA is to infer for each SNP in disease their posterior probability of disease association and to detect functional enrichments or depletions from the annotations, taking into account the underlying multi-trait epigenomic covariance.

#### Input
1. GWAS summary association statistics in one or more traits (Z-scores)
2. Linkage disequilibrium (LD) either from the GWAS cohort or reference panel from 1000 Genome consortium
3. Functional annotation matrix (binary or continuous) for each SNP

#### Important features
1. Efficient full Bayesian inference of causal SNP and causal annotations allows incorporation of large number of annotations
2. Can model epigenomic covariance of multiple related traits (model complexity is linear to the number of traits)
3. Efficient posteior inference of causal configuration automatically determines the number of causal variants
4. Simutaneously model the underlying heritability parameters (variance explained per SNP) and leverage it in causal inference

## Installation
RiVIERA requires Rcpp and RcppArmadillo, which can be easily installed within R via 'install.packages' function.

Download and install:

`$ git clone https://github.com/yueli-compbio/RiVIERA-MT`

Mac installation:

`$ R CMD INSTALL RiVIERA_0.9.3_MacOS.tgz`

Linux installation:

`$ R CMD INSTALL RiVIERA_0.9.3_Linux.tar.gz`

## Documentation
Function manuals are described in R documents:

`> library(RiVIERA)`

`> ?RiVIERA`

User manual with examples is written in sweave and invoked by vignette:

`> vignette(RiVIERA)`

