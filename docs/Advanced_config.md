# Here are some advanced configuration options for Nextflow
# Resources (Memory/CPUs...)
Some of the process in the pipeline are extremely power hungry & time consuming at the sametime. The pipeline was "preconfiged" based on our testing at [Agriculture Victoria](https://www.agriculture.vic.gov.au/). However, you can change the resource allocation for each process by editing the `nextflow.config` file. For example, a problem arise if you want to do short-read polishing as the kmer estimation with `LongFilt` is extremely time & resource consuming, you can increase the allocation for `LongFilt` from 128GB to 256GB by editing the `nextflow.config` file 