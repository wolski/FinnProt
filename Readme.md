## install the FinnProt R package

```{r}
install.packages('devtools')
library(devtools)
install_git('https://github.com/wolski/FinnProt', build_vignettes = TRUE, quiet = FALSE)
```

## build the ISCB2017 R package

```{r}
roxygen2::roxygenise()
```


## read the vignettes

```{r}
# get an overview
library(FinnProt)

vignette(package="FinnProt")
vignette('fdr2')
```
