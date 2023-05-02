# &#19918; <img align="right" width="300" src="https://github.com/sunyatin/qna_data/blob/main/model.png">

This repository contains all relevant simulated data[^1] from the study "*Questioning Neanderthal admixture*" (doi: https://doi.org/10.1101/2023.04.05.535686). Scripts and additional files are found in another repository named [qna](https://github.com/sunyatin/qna).

It also contains, within `genetic_maps/`, the empirical recombination maps (PLINK HapMap, Spence et al. 2019) used in the study.

# Layout

Details about the files can be found in the README of the respective directories.

```bash
Final_Blake/		# archive of the simulated data
	data/		# simulated data
	further/	# further simulations (aDNA, Fst trajectories...)

genetic_maps/		# empirical genetic maps
	HapMap/
	Spence19/
```

[^1]: Genetic data are in [EIGENSTRAT](https://reich.hms.harvard.edu/software/InputFileFormats) format with a modification: `0` encodes the **ancestral homozygous** genotype (instead of the *derived* homozygous genotype in pure EIGENSTRAT). Subsequently, `2` encodes the derived homozygous genotype. All genotypes are mono- or bi-allelic at most.
