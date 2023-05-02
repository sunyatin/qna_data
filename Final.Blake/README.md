# Description of the directory content

**Note.** Genome sizes are written as AxB with A the number of chromosomes and B their size in Mbp.

### **data**

Files in this directory were generated using the [`general.sh`](https://github.com/sunyatin/qna/blob/main/general.sh) script.


| Directory | Description | Genome size | Recombination type | Content |
| -- | -- | -- | -- | -- |
| `1M` | Genetic data simulated from sampling one million times in the parameter prior distributions, after statistical screening | 10x7 | Uniform | par+stats |
| `20x30Mbp.1_2e-8` | The published admixture models (1 run/model) simulated with a fixed mutation rate of 1.2e-8 | 20x30 | Uniform | par+stats |
| `20x30Mbp.50sim` | The published admixture models (50 runs/model with variable mutation rate) and our structured model (20 accepted runs) | 20x30 | Uniform | par+stats |
| `20x30Mbp.50sim.HOTSPOTS` | The published admixture models (50 runs/model with variable mutation rate) and our structured model (20 accepted runs) | 20x30 | Hetero. | par+stats |
| `20x30Mbp` | Our structured model (20 accepted runs) | 20x30 | Uniform | par+data+stats |
| `empirical_gmaps` | Run 1014230 of our structured model simulated under empirical genetic maps (HapMap and Spence19) | 20x50 | Empirical | par+stats |
| `param_prior_sampling` | Subset of 5,716 parameter files to suggest the raw distribution of tested parameter combinations | N/A | N/A | par files |


### **further**

Files in this directory were generated using the [`further.sh`](https://github.com/sunyatin/qna/blob/main/further.sh) script.

| Directory | Description | Genome size | Recombination type | Content |
| -- | -- | -- | -- | -- |
| `20x30Mbp.U.CEU3` | aDNA simulations, sampling Eurasians in the 3rd (0-based indexing) deme of the Eurasian metapopulation <ul><li>`stats_aDNA.di.1M` analyzed as diploid genotypes for 1M SNPs</li><li>`stats_aDNA.di.All` analyzed as diploid genotypes for all SNPs</li><li>`stats_aDNA.pseudodi.1M` analyzed as pseudodiploid genotypes for 1M SNPs</li><li>`stats_aDNA.pseudodi.Archaic` analyzed as pseudodiploid genotypes for SNPs with "Archaic" ascertainment (cf. SupMat)</li></ul> | 20x30 | Uniform | par+stats |
| `Fst_traj_*A*_*B*` | $F_{ST}$ values simulated for run 1014230 between populations *A* and *B* (0-based index). The name of the file is the time of individual sampling in years BP | 10x7 | Uniform | par+stats |
| `LD_implementation` | Simulations to compare the decay constant of the ancestry-LD curves estimated using `computed` and our implementation | 10x10 | Uniform | par+data+stats |
| `sensitivity` | Various simulations for robustness assessment | 20x30 | Uniform | par+stats |
