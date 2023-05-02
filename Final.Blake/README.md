# Description of the directory content

**Note.** Genome sizes are written as {*A*}x{*B*} with *A* the number of chromosomes and *B* their size in Mbp.

### **data**

Files in this directory were generated using the [`general.sh`](https://github.com/sunyatin/qna/blob/main/general.sh) script.


| Directory | Description | Genome size | Recombination type | Content |
| -- | -- | -- | -- | -- |
| `1M` | Genetic data retained post-statistical screening, simulated after sampling one million times in the parameter prior distributions | 10x7 | Uniform | par+stats |
| `20x30Mbp.1_2e-8` | The published admixture models (1 run/model) simulated with a fixed mutation rate of 1.2e-8 | 20x30 | Uniform | par+stats |
| `20x30Mbp.50sim` | The published admixture models (50 runs/model with variable mutation rates) and our structured model (20 accepted runs) | 20x30 | Uniform | par+stats |
| `20x30Mbp.50sim.HOTSPOTS` | The published admixture models (50 runs/model with variable mutation rate) and our structured model (20 accepted runs) | 20x30 | Heterogeneous | par+stats |
| `20x30Mbp` | Our structured model (20 accepted runs) | 20x30 | Uniform | par+data+stats |
| `empirical_gmaps` | Run 1014230 of our structured model simulated under empirical genetic maps (HapMap and Spence19) | 20x50 | Empirical | par+stats |
| `param_prior_sampling` | Subset of 5,716 parameter files to suggest the raw distribution of the sampled parameters | N/A | N/A | par |


### **further**

Files in this directory were generated using the [`further.sh`](https://github.com/sunyatin/qna/blob/main/further.sh) script.

| Directory | Description | Genome size | Recombination type | Content |
| -- | -- | -- | -- | -- |
| `20x30Mbp.U.CEU3` | aDNA simulations, sampling Eurasians in the 3rd (0-based indexing) deme of the Eurasian metapopulation:<br><br> <ul><li>`stats_aDNA.di.1M` analyzed as diploid genotypes for 1M SNPs</li><li>`stats_aDNA.di.All` analyzed as diploid genotypes for all SNPs</li><li>`stats_aDNA.pseudodi.1M` analyzed as pseudodiploid genotypes for 1M SNPs</li><li>`stats_aDNA.pseudodi.Archaic` analyzed as pseudodiploid genotypes for SNPs with "Archaic" ascertainment (cf. SupMat)</li></ul>**Files are written as:<br> {*RunID*}__aDNA.{*MetaPop*}.{*DemeID*}.{*SamplingTimeYearsAgo*}** | 20x30 | Uniform | par+stats |
| `20x30Mbp.U.CEU3` | aDNA simulations, same as before, but sampling ancient Eurasians at the relative sampling location of the original model and using only diploid genotypes with all SNPs. **This directory also includes aDNA simulations under the Schaefer et al. (2021) model** | 20x30 | Uniform | par+stats |
| `Fst_traj_{A}_{B}` | $F_{ST}$ values simulated under run 1014230 between demes (or extreme-ends of metapopulations) *A* and *B* (0-based index). The names of the files are the sampling ages (years BP) | 10x7 | Uniform | par+stats |
| `LD_implementation` | Simulations to compare the decay constant of the ancestry-LD curves estimated using `computed` and our python implementation | 10x10 | Uniform | par+data+stats |
| `sensitivity` | Various simulations for robustness assessment | 20x30 | Uniform | par+stats |
