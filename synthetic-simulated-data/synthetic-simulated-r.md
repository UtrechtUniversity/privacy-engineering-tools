# R Packages To Generate Synthetic Data & Simulated Data

Below is a selection of R packages which allow to create (mostly tabular) synthetic datasets. We divided the packages into three categories: purely generative datasets, not purely generative (i.e., based on input data), and packages for specific use-cases. This is a loose classification, since packages might fall into multiple categories.

For more inspiration on how to create fake data in R, see [this Rstudio blogpost](https://rviews.rstudio.com/2020/09/09/fake-data-with-r/).

## Generative

The following packages can generate synthetic data without the need for any input data to generate the synthetic dataset from (listed alphabetically):

| Name | Description | More info | Maintenance | GitHub stars |
|---|---|---|---|---|
| [charlatan](https://cran.r-project.org/web/packages/charlatan/index.html) | Generation of fake data, e.g., names, dates, addresses, etc. | [Documentation](https://docs.ropensci.org/charlatan/), [GitHub](https://github.com/ropensci/charlatan) | Active | 100-500
| [conjurer](https://cran.r-project.org/web/packages/conjurer/index.html) | A Parametric Method for Generating Synthetic Tabular Data | [Documentation](https://www.foyi.co.nz/posts/documentation/documentationconjurer/), [GitHub](https://github.com/SidharthMacherla/conjurer) | Active | 0-10
| [fabricatr](https://cran.r-project.org/web/packages/fabricatr/index.html) | Simulate hierarchical data structures and correlated data (tabular), either from random number generators or by resampling from existing data sources | [Documentation](https://declaredesign.org/r/fabricatr/), [GitHub](https://github.com/DeclareDesign/fabricatr) | Active | 10-100
| [faux](https://cran.r-project.org/web/packages/faux/index.html) | Create datasets with factorial structure through simulation by specifying variable parameters | [Documentation](https://debruine.github.io/faux/), [Published version](https://doi.org/10.5281%2Fzenodo.2669586), [GitHub](https://github.com/debruine/faux) | Active | 10-100
| [simPop](https://cran.r-project.org/web/packages/simPop/index.html) | Simulation of populations for surveys based on auxiliary data (model-based, calibration, combinatorial optimization) | [Article](https://doi.org/10.18637%2Fjss.v079.i10), [documentation](https://cran.r-project.org/web/packages/simPop/simPop.pdf), [GitHub](https://github.com/statistikat/simPop) | Active | 10-100
| [wakefield](https://cran.r-project.org/web/packages/wakefield/index.html) | Generates random dataframes, lists and vectors from a selection of variable types (e.g., age, sex, date, religion, zip code, etc.) | [Documentation](https://cran.r-project.org/web/packages/wakefield/wakefield.pdf), [GitHub](https://github.com/trinker/wakefield) | Inactive | 100-500

## Not purely generative

The following packages use/need some kind of input dataset to generate the synthetic dataset from (listed alphabetically):

| Name | Description | More info | Maintenance | GitHub stars |
|---|---|---|---|---|
| [mice](https://cran.r-project.org/web/packages/mice/index.html) | Extend imputation procedures for missing data to synthetic data, such that (part of) the observed data can be easily overimputed with fake, privacy-preserving, synthetic records | [Documentation](https://www.gerkovink.com/miceVignettes/synthetic/synthetic.html), [article](https://doi.org/10.3390/psych3040045), [GitHub](https://github.com/amices/mice) | Active | 100-500
| [synthesis](https://cran.r-project.org/web/packages/synthesis/index.html) | Generate Synthetic time series from commonly used statistical models (e.g., linear, nonlinear, chaotic systems) | [Documentation](https://cran.r-project.org/web/packages/synthesis/vignettes/synthesis.html) [article](https://doi.org/10.1016%2Fj.advwatres.2019.103430), [GitHub](https://github.com/zejiang-unsw/synthesis) | Active | 0-10
| [synthpop](https://cran.r-project.org/web/packages/synthpop/index.html) | Produces synthetic versions of tabular microdata containing confidential information with minimal distortion of statistical information (using sequential modelling) | [Documentation](https://www.synthpop.org.uk/), [article](https://doi.org/10.18637/jss.v074.i11), [GitHub](https://github.com/bnowok/synthpop) | Active | 10-100

## Specific use-cases

The following packages were developed for specific use-cases and are not purely generative (listed alphabetically):

| Name | Description | More info | Maintenance | GitHub stars |
|---|---|---|---|---|
| [NestedCategBayesImpute](https://cran.r-project.org/web/packages/NestedCategBayesImpute/index.html) | Modeling, Imputing and Generating Synthetic Versions of Nested Categorical Data in the Presence of Impossible Combinations | [Documentation](https://cran.r-project.org/web/packages/NestedCategBayesImpute/NestedCategBayesImpute.pdf) | - | - 
| [synthACS](https://cran.r-project.org/web/packages/synthACS/index.html) | Access American Community Survey (ACS) data, build synthetic ACS microdata at any specified geographical level, add additional attributes to the synthetic dataset, and conduct spatial microsimulation modelling (SMSM) | [Documentation](https://cran.r-project.org/web/packages/synthACS/vignettes/jss_synthACS.pdf), [article](https://doi.org/10.18637%2Fjss.v104.i07), [GitHub](https://github.com/alexWhitworth/synthACS) | Active | 0-10
