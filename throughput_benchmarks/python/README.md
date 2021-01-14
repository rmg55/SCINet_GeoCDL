### Benchmarking Remote Datasets with Python

To test the scalability and throughput associated with different file-types and remote data stores, we use a compbination of:
1. Dask Distributed
2. Dask Arrays
3. fsspec (and associated remote file systems)

Much of the code / architecture was re-used and inspired by a similiar effort in the Pangeo community ([see this link](http://gallery.pangeo.io/repos/earthcube2020/ec20_abernathey_etal/cloud_storage.html) or this [preprint](https://www.authorea.com/doi/full/10.22541/au.160443768.88917719/v1)).

To perform a benchmark:

1. Make of Copy of the template file and rename.
2. Fill in the associated code to access the data as a Dask Array in the "*Dataset Specific IO Code*" section.
3. Fill in the metadata in the "*Dataset Specific IO Code*" section.
4. Run notebook on Ceres / Atlas / etc...
5. If completed successfully, results will be pushed to the `../results` folder.
5. Send Pull request with the new file in the `../results` folder and the new Jupyter Notebook with the analysis.

Computational Environment:

Code be run in this docker containers:

https://hub.docker.com/r/rowangaffney/data_science_im_rs

or can be run in a conda environment with the correct packages installed.