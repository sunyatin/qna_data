# Description of the directory content

**Note.** Genome sizes are written as AxB with A the number of chromosomes and B their size in Mbp.

**data**

| Directory | Description | Genome size | Recombination type | Content |
| -- | -- | -- | -- | -- |
| `1M` | Genetic data simulated from sampling one million times in the parameter prior distributions, after statistical screening | 10x7 | Uniform | par + stats |
| `20x30Mbp.1_2e-8` | The published admixture models (1 run/model) simulated with a fixed mutation rate of 1.2e-8 | 20x30 | Uniform | par + stats |
| `20x30Mbp.50sim` | The published admixture models (50 runs/model with variable mutation rate) and our structured model (20 accepted runs) | 20x30 Mbp | Uniform | par + stats |
| `20x30Mbp.50sim.HOTSPOT`S | The published admixture models (50 runs/model with variable mutation rate) and our structured model (20 accepted runs) | 20x30 | Hetero. | par + stats |
| `20x30Mbp` | Our structured model (20 accepted runs) | 20x30 | Uniform | all (incl. data) |
| `empirical_gmaps` | Run 1014230 of our structured model simulated under empirical genetic maps (HapMap and Spence19) | 20x50 | Empirical | par + stats |
| `param_prior_sampling` | Subset of 5,716 parameter files to suggest the raw distribution of tested parameter combinations | N/A | N/A | par files |


**further**

| Directory | Description | Genome size | Recombination type | Content |
| -- | -- | -- | -- | -- |
| `20x30Mbp.U.CEU3` | <ul><li>item1</li><li>item2</li></ul> | . | . | . |
