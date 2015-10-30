# ph_datasets
Persistent Homology Datasets

Collected datasets used in publications applying persistent homology to problems in genomics by the Rabadan Lab.

##### Chan, J., Carlsson, G., and Rabadan, R. Topology of viral evolution. _Proceedings of the National Academy of Sciences_ 110.46 (2013) 18566-18571. [[link]](http://www.pnas.org/content/110/46/18566.abstract)

* `pnas2013/avian_HA_nt_concat_jukes_cantor.csv`: HA segment of influenza. Will have trivial topology. Provided as a distance matrix using a Jukes-Cantor metric arranged lower diagonal, column wise. [output of Matlab's `seqpdist`]
* `pnas2013/avian_all_nt_concat_jukes_cantor.csv`: Concatenated segments of influenza. Will have nontrivial topology. Provided as a distance matrix using Jukes-Cantor metric arranged lower diagonal, column wise. [output of Matlab's `seqpdist`]
* `pnas2013/avian_NA_nt_concat_jukes_cantor.csv`: NA segment of influenza. Will have trivial topology. Provided as a distance matrix using a Jukes-Cantor metric arranged lower diagonal, column wise. [output of Matlab's `seqpdist`]

* HIV Dataset

##### Emmett, K., Rosenbloom, D., Camara, P., Rabadan, R. Parametric Inference Using Persistence Diagrams: A Case study in Population Genetics. _ICML Workshop on Topological Methods in Machine Learning_ (2014). [[arXiv]](http://arxiv.org/abs/1406.4582)

Results in this paper relied on coalescent simulations generated using [`ms`](http://home.uchicago.edu/rhudson1/source/mksamples.html).
We provide two sample datasets, one with recombination and one without.

* `icml2014/ms_n100_t500_r100`: With recombination. 100 samples, scaled mutation rate 500 and scaled recombination rate recombination of 100. Provided as a binary sequence matrix.
* `icml2014/ms_n100_t500_r0`: No recombination. 100 samples, scaled mutation rate 500 and no recombination. Provided as a binary sequence matrix.

##### Emmett, K., and Rabadan, R. Characterizing Scales of Genetic Recombination and Antibiotic Resistance in Pathogenic Bacteria Using Topological Data Analysis. _Lecture Notes in Computer Sciences_ 540--551 (2014). [[arXiv]](http://arxiv.org/abs/1406.1219)

* Bacteria MLST
* Bacteria PATRIC 

##### Camara, P. G., Levine, A. J. and Rabadan, R. Inference of ancestral recombination graphs through topological data analysis. [[arXiv]](http://arxiv.org/abs/1505.05815)

* `TARGet/Darwin_Finches.fa`: 112 Darwin's finches from Galapagos Islands. Provided as a FASTA file with the genetic variation of 142 homozygous bi-allelic SNPs present in a 9 Mb scaffold.
* `TARGet/Divergent_Populations_Isolated.fa`: 300 sequences with 300 segregating sites, sampled from two populations with sample sizes N and 0.2N, that diverged 24N generations before present. The scaled recombination rate is 40. 250 sequences are sampled from the first population and 50 from the second one. The sequences were generated using coalescent simulations with software [`ms`](http://home.uchicago.edu/rhudson1/source/mksamples.html).
* `TARGet/Divergent_Populations_Migration.fa`: Same as the previous set but with mutation rate between the two populations equal to 2N.

#### ms: large-scale ms simulations

Large-scale ms simulations for persistent homology algorithm development. Provided as binary matrix.

* `ms/n5000`: generated with `ms 5000 1 -t 200 -r 200 500000`
* `ms/n10000`: generated with `ms 10000 1 -t 200 -r 200 500000`
* `ms/n20000`: generated with `ms 20000 1 -t 200 -r 200 500000`
