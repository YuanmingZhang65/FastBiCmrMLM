FastBiCmrMLM (Fast Binary-trait Compressed variance component multi-locus random-SNP-effect Mixed Logistic Model) is an R package designed for case-control genome-wide association study (GWAS), which consider additive and dominant effects and their polygenic backgrounds in a compressed variance component mixed logistic model.

The current version, FastBiCmrMLM v0.0.1, features four algorithms:
1) FastBiCmrMLM: Primary algorithm for FastBiCmrMLM, which is used to analyze small samples with the number of individuals less than 1,000.
2) FastBiCmrMLM-Time: A fast version of FastBiCmrMLM, which is used to analyze the samples with the number of individuals from 1,000 to 20,000. FastBiCmrMLM-Time took about seven minutes for one disease of WTCCC1 datasets.
3) FastBiCmrMLM-RAM: Optimized for memory efficiency, which is used to save memory when sample size is large (≥ 20,000). In the analysis of biobank-scale simulation datasets (500,000 individuals and one million SNP markers), FastBiCmrMLM-RAM took about 13.5 hours on the server with 10 CPUs and the memory usage of 141 Gb for one sample.
4) FastBiCmrMLM-Hap: Haplotypes for each bin are constructed by adjacent linkage disequilibrium markers and used to associate the trait of interest using FastBiCmrMLM.

Algoirthms 1) to 3) can be used to detect structure variant. FastBiCmrMLM v0.0.1 works only on Linux system.

Please cite the paper: Wang JT, Chang XY, Zhao Q, and Zhang YM. FastBiCmrMLM: a fast and powerful compressed variance component mixed logistic model for big genomic case-control genome-wide association study. Brief Bioinform, 2024, 25: bbae290. DOI: 10.1093/bib/bbae290
