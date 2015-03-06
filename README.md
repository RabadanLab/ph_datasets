# ph_datasets
Persistent Homology Datasets

Collected datasets used in publications applying persistent homology to problems in genomics by the Rabadan Lab.

##### Chan, J., Carlsson, G., and Rabadan, R. Topology of viral evolution. _Proceedings of the National Academy of Sciences_ 110.46 (2013) 18566-18571. [[link]](http://www.pnas.org/content/110/46/18566.abstract)

* `pnas2013/avian_HA_nt_concat_jukes_cantor.csv`: HA segment of influenza. Will have trivial topology. Provided as a distance matrix using a Jukes-Cantor metric arranged as a row vector.
* `pnas2013/avian_all_nt_concat_jukes_cantor.csv`: Concatenated segments of influenza. Will have nontrivial topology. Provided as a distance matrix using Jukes-Cantor metric arranged as a row vector.

* HIV Dataset

##### Emmett, K., Rosenbloom, D., Camara, P., Rabadan, R. Parametric Inference Using Persistence Diagrams: A Case study in Population Genetics. _ICML Workshop on Topological Methods in Machine Learning_ (2014). [[arXiv]](http://arxiv.org/abs/1406.4582)

Results in this paper relied on coalescent simulations generated using [`ms`](http://home.uchicago.edu/rhudson1/source/mksamples.html).
We provide two sample datasets, one with recombination and one without.

* `icml2014/ms_n100_t500_r100`: With recombination. 100 samples, scaled mutation rate 500 and scaled recombination rate recombination of 100. Provided as a binary sequence matrix.
* `icml2014/ms_n100_t500_r0`: No recombination. 100 samples, scaled mutation rate 500 and no recombination. Provided as a binary sequence matrix.

##### Emmett, K., and Rabadan, R. Characterizing Scales of Genetic Recombination and Antibiotic Resistance in Pathogenic Bacteria Using Topological Data Analysis. _Lecture Notes in Computer Sciences_ 540--551 (2014). [[arXiv]](http://arxiv.org/abs/1406.1219)

* Bacteria MLST
* Bacteria PATRIC 
