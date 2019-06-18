Functions for writing commands and post processing the MiXCR pipeline.

Given a sample data matrix that indicates the sample name, sample folder name and input paths
this script can write out pipeline commands to run MiXCR on the cluster and post process the
data.


## Assembling this package
In R:
``` r
housekeeping::assemble_package(package_name = "MiXCR", my_version = "0.0-01",
  my_dir = "/datastore/alldata/shiny-server/rstudio-common/dbortone/packages/MiXCR")
```

## Push changes
In bash:
``` bash
cd /datastore/alldata/shiny-server/rstudio-common/dbortone/packages/MiXCR
my_comment="Assembled package."
git commit -am "$my_comment"; git push origin master
git tag -a 0.0-01 -m "$my_comment"; git push -u origin --tags
```

## Install
Restart R
In R (local library, packrat library):
``` r
devtools::install_github("DanteBortone/MiXCR")
```

Or for a specific version:
``` r
devtools::install_github("DanteBortone/MiXCR", ref = "0.0-01")
```