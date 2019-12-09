
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Plotnine: Grammar of Graphics for Python

A translation of the visualisation chapters from “R for Data Science” to
Python using Plotnine and Pandas.

## R packages used

``` r
session_info()
```

    ─ Session info ───────────────────────────────────────────────────────────────
     setting  value                       
     version  R version 3.6.1 (2019-07-05)
     os       macOS Mojave 10.14.6        
     system   x86_64, darwin15.6.0        
     ui       X11                         
     language en_US.UTF-8                 
     collate  en_US.UTF-8                 
     ctype    en_US.UTF-8                 
     tz       Europe/Amsterdam            
     date     2019-12-09                  
    
    ─ Packages ───────────────────────────────────────────────────────────────────
     ! package     * version date       lib source        
     P assertthat    0.2.1   2019-03-21 [?] CRAN (R 3.6.0)
     P cli           1.1.0   2019-03-19 [?] CRAN (R 3.6.0)
     P crayon        1.3.4   2017-09-16 [?] CRAN (R 3.6.0)
     P digest        0.6.23  2019-11-23 [?] CRAN (R 3.6.0)
     P evaluate      0.14    2019-05-28 [?] CRAN (R 3.6.0)
     P htmltools     0.4.0   2019-10-04 [?] CRAN (R 3.6.0)
     P jsonlite      1.6     2018-12-07 [?] CRAN (R 3.6.0)
     P knitr       * 1.26    2019-11-12 [?] CRAN (R 3.6.0)
     P lattice       0.20-38 2018-11-04 [?] CRAN (R 3.6.0)
     P magrittr      1.5     2014-11-22 [?] CRAN (R 3.6.0)
     P Matrix        1.2-18  2019-11-27 [?] CRAN (R 3.6.0)
     P Rcpp          1.0.3   2019-11-08 [?] CRAN (R 3.6.0)
     P renv          0.9.1   2019-12-09 [?] CRAN (R 3.6.1)
     P reticulate  * 1.13    2019-07-24 [?] CRAN (R 3.6.0)
     P rlang         0.4.2   2019-11-23 [?] CRAN (R 3.6.0)
     P rmarkdown     1.18    2019-11-27 [?] CRAN (R 3.6.0)
     P sessioninfo * 1.1.1   2018-11-05 [?] CRAN (R 3.6.0)
     P stringi       1.4.3   2019-03-12 [?] CRAN (R 3.6.0)
     P stringr       1.4.0   2019-02-10 [?] CRAN (R 3.6.0)
     P withr         2.1.2   2018-03-15 [?] CRAN (R 3.6.0)
     P xfun          0.11    2019-11-12 [?] CRAN (R 3.6.0)
     P yaml          2.2.0   2018-07-25 [?] CRAN (R 3.6.0)
    
    [1] /Users/jeroen/repos/datascienceworkshops/r4ds-python-plotnine/renv/library/R-3.6/x86_64-apple-darwin15.6.0
    [2] /private/var/folders/8h/88ch3k996hb0t11db8bj9pzh0000gn/T/RtmpdFCOov/renv-system-library
    
     P ── Loaded and on-disk path mismatch.

## Python packages used

``` bash
. venv/bin/activate && pip freeze
```

    adjustText==0.7.3
    appnope==0.1.0
    attrs==19.3.0
    backcall==0.1.0
    bleach==3.1.0
    cycler==0.10.0
    decorator==4.4.1
    defusedxml==0.6.0
    descartes==1.1.0
    entrypoints==0.3
    importlib-metadata==1.2.0
    ipykernel==5.1.3
    ipython==7.10.1
    ipython-genutils==0.2.0
    ipywidgets==7.5.1
    jedi==0.15.1
    Jinja2==2.10.3
    joblib==0.14.0
    jsonschema==3.2.0
    jupyter==1.0.0
    jupyter-client==5.3.4
    jupyter-console==6.0.0
    jupyter-core==4.6.1
    jupytext==1.3.0
    kiwisolver==1.1.0
    MarkupSafe==1.1.1
    matplotlib==3.1.2
    mistune==0.8.4
    mizani==0.6.0
    more-itertools==8.0.2
    nbconvert==5.6.1
    nbformat==4.4.0
    notebook==6.0.2
    numpy==1.17.4
    palettable==3.3.0
    pandas==0.25.3
    pandocfilters==1.4.2
    parso==0.5.1
    patsy==0.5.1
    pexpect==4.7.0
    pickleshare==0.7.5
    plotnine==0.6.0+23.g3eb58cd
    prometheus-client==0.7.1
    prompt-toolkit==2.0.10
    ptyprocess==0.6.0
    Pygments==2.5.2
    pyparsing==2.4.5
    pyrsistent==0.15.6
    python-dateutil==2.8.1
    pytz==2019.3
    PyYAML==5.2
    pyzmq==18.1.1
    qtconsole==4.6.0
    scikit-learn==0.22
    scikit-misc==0.1.1
    scipy==1.3.3
    Send2Trash==1.5.0
    six==1.13.0
    statsmodels==0.10.2
    terminado==0.8.3
    testpath==0.4.4
    tornado==6.0.3
    traitlets==4.3.3
    wcwidth==0.1.7
    webencodings==0.5.1
    widgetsnbextension==3.5.1
    zipp==0.6.0
