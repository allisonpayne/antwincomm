
<!-- README.md is generated from README.Rmd. Please edit that file -->

# antwincomm

<!-- badges: start -->
<!-- badges: end -->

Characterizing the marine winter predator community (seabirds and marine
mammals) around the northern Antarctic Peninsula (including the
Bransfield Strait and South Shetland Islands) using observations
collected during the 2012-2016 NOAA/NSF austral winter cruises on the RV
Ice Breaker Nathaniel B. Palmer. 



*Work in progress!!*

## Code

All code under development for **antwincomm** can be found in this
repository. The analysis pipeline [uses
`targets`](https://books.ropensci.org/targets/) to manage workflow
caching and dependencies. Better documentation to follow (promise). This
repository will be archived on Zenodo or somewhere similar at
publication.

## Data

The **antwincomm** data are too large for GitHub, so they’re stored in
the [antwincomm Open Science Framework project](https://osf.io/hwnvy/).
Currently private, will be made public no later than time of
publication. For access to the OSF project, please contact Max
Czapanskiy (max \[dot\] czapanskiy \[at\] noaa \[dot\] gov).

For the code to work, you must download data/WAMLR from the OSF project
into data/WAMLR in your local copy of the repository. You can do that
manually or by running the following lines of code. Until the project is
made public, though, you’ll first have to [authenticate
`osfr`](https://docs.ropensci.org/osfr/articles/auth.html).

``` r
dir.create(here::here("data"))
osf_wamlr <- osfr::osf_retrieve_file("6407bf6228e5c503cc9376b3")
osfr::osf_download(osf_wamlr, path = here::here("data"), recurse = TRUE)
```

## Outputs

See the [project website](https://flukeandfeather.github/io/antwincomm)
for a list of reports documenting the analysis pipeline.
