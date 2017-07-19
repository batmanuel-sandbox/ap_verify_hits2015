# verify_ap_hits2015
Data from HiTS (2015) to verify the performance of alert production in the LSST DM stack.

This repo is designed to be used as a template for developing new data sets for integration into `verify_ap`.

It is currently set up for using `obs_test`.

Relevant Files and Directories
-----
path                  | description
:---------------------|:-----------------------------
`raw`                 | To be populated with photometrically and astrometrically calibrated data. Currently contains a single small fits file (taken from `obs_test`) to test `git-lfs` functionality.
`calib`               | To be populated with master calibs. Currently empty.
`templates`           | To be populated with calibrated images intended to be used as templates. Currently empty.
`data`                | Butler repo into which raw data can be ingested.  This should be copied to an appropriate location before ingestion.  Note that the `_mapper` file will require updating for other instruments.
`ref_cats`            | To be populated with relevant reference catalogs. Currently empty.
`dataIds.list`        | List of dataIds in this repo. For use in running Tasks. Currently set to run all Ids.


Git LFS
-------

To clone and use this repository, you'll need Git Large File Storage (LFS).

Our [Developer Guide](http://developer.lsst.io/en/latest/tools/git_lfs.html) explains how to setup Git LFS for LSST development.

