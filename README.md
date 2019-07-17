### Clone- and haplotype specific cancer karyotypes inferred with RCK ([paper](https://www.biorxiv.org/content/10.1101/560839v1)|[code](https://github.com/aganezov/RCK)) on 17 prostate cancer samples

Directories are organized as follows:

````
  sample/cna/sample_cna-fp.rck.(a|s)cnt.tsv
````

where:
* `sample` -- sample identifyer (e.g., `A10c`, where `A10` is the patient id in the original paper ([link](https://www.nature.com/articles/nature14347)) and `c` is the sample from the respective patient).
* `cna`    -- input allele-specific segment copy number tensor from either Battenberg or HATCHet.
* `fp`     -- False Positive paramter for the input Novel Adjacenceis utilization (i.e., reconstrcuted keryotypes must have at least `1-fp` fraction of input Novel Adjacencies being present across all the clones in the sample)

`acnt` determines the adjacency copy number tensor, with copy numbers for every input novel adjacency (labeled versions) in every clone, as well as for every reference adjacency.

`scnt` determines the segment copy number tensor with clone- and haplotype-specific copy numbers.

For more information on both segment and adjacency copy number tensors formats, please, refer to the original [RCK repository "results" section](https://github.com/aganezov/RCK#results).

