# amaendle.r-universe.dev

This contains the index for the [r-universe repository](https://amaendle.r-universe.dev/builds).  
The R-universe project provides an alternative package repository ecosystem including automated package builds and checks outside of the familiar CRAN or BioConductor infrastructure.  
Aside from the discoverability bonus (see e.g. the [R-universe landing page](https://r-universe.dev/)), the additional build system also allows package installation via `install.packages()`:

You can install the current development version of a package from GitHub and built by R-universe like this:

```r
install.packages("PUcopula", repos = "https://amaendle.r-universe.dev")
```

## Maintaining this universe

See [the r-universe docs](https://docs.r-universe.dev/publish/set-up.html) for the general setup procedure.

To add new packages, edit [`packages.json`](packages.json) accordingly (make sure it's syntactically valid JSON).  
For CRAN packages, [adding them here should not be necessary](https://docs.r-universe.dev/publish/set-up.html#populating-the-packages.json-registry-file), 
but for completeness it is likely a good idea to keep track of packages anyway, in particular if you want to make development versions accessible more easily.
