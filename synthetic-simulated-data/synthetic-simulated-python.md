# Python packages to create synthetic data

This is a list of Python packages that can help you generate synthetic data. The list was compiled mainly through searching in Google and GitHub. Naturally, some packages will be missing, so feel free to suggest other packages via a Pull Request.

We divided the packages into three categories: Tabular dataset, Purely generative datasets and packages for specific use cases. This is a loose classification, since packages might fall into multiple categories.

## Tabular datasets

This packages in this category are useful if you have a tabular dataset and want to create a new synthetic dataset with similar properties (listed in alphabetical order).

| Name | Methods |  Extra Features | Synthetic spectrum | More info | License | Maintenance | GitHub stars
|--|--|--|--|--|--|--|--|
| [DataSynthesizer](https://github.com/DataResponsibly/DataSynthesizer) | Bayesian Network | Web User Interface, intermediate file, differential privacy | Synthetic structural, synthetically-augmented plausible, synthetically-augmented multivariate plausible | [Article](https://github.com/DataResponsibly/DataSynthesizer/blob/master/docs/cr-datasynthesizer-privacy.pdf) | MIT | Active | 100-500
| [Gretel Synthetics](https://github.com/gretelai/gretel-synthetics) | LSTM | Differential Privacy | Synthetically-augmented multivariate plausible | - | [Apache-2.0](https://github.com/gretelai/gretel-synthetics/blob/master/LICENSE) | Active | 100-500
| [Synthetic Data Vault](https://github.com/sdv-dev/SDV) (SDV) | Copula, GAN, TVAE | Single table, relational database, time-series, de-identification | Synthetically-augmented replica | [Article](https://doi.org/10.1109/DSAA.2016.49) ([pdf](https://dai.lids.mit.edu/wp-content/uploads/2018/03/SDV.pdf)), [documentation](https://sdv.dev/SDV/) | [MIT](https://github.com/sdv-dev/SDV/blob/master/LICENSE) | Active | 500-1000
| [synthia](https://github.com/dmey/synthia) | fPCA, Gaussian copula, vine copula | Supports xarray | Synthetically-augmented multivariate/univariate plausible| [software](https://doi.org/10.21105/joss.02863), [application](https://doi.org/10.5194/gmd-14-5205-2021) | MIT | Active | 10-100
| [ydata-synthetic](https://github.com/ydataai/ydata-synthetic) | GAN | Single table and time-series | Synthetically-augmented multivariate plausible | - | [MIT](https://github.com/ydataai/ydata-synthetic/blob/dev/LICENSE) | Active | 500-1000

## Generative

Generative methods generally do not need any input dataset. Instead, the user specifies the properties of the dataset and the package generates the synthetic data from this specification (listed in alphabetical order).

| Name | Data type | Extra features | More info |  License | Maintenance | GitHub stars |
|--|--|--|--|--|--|--|
| [BlenderProc](https://github.com/DLR-RM/BlenderProc) | Images for segmentation, distance estimation  |  Physics simulation, camera sampling | [Article](https://doi.org/10.48550/arXiv.1911.01911) | GPL-v3 | Active | 1K+ |
| [faker](https://github.com/joke2k/faker) | Many kinds of private information | Modular structure | - |  MIT | Active | 10K+
| [google-semantic-location-history](https://github.com/UtrechtUniversity/google-semantic-location-history) | Google semantic location histories | - | - | MIT | Active | 2 |
| [mimesis](https://github.com/lk-geimfari/mimesis) | Many kinds of private information | High performance, multilingual | -  | MIT | Active | 3k+ |
| [physim-dataset-generator](https://github.com/cmitash/physim-dataset-generator) | Images for object detection | 3D rendering | [Article](https://doi.org/10.1109/IROS.2017.8202206) | [BSD-2-Clause](https://github.com/cmitash/physim-dataset-generator/blob/master/LICENSE) | Inactive | 60+ |
| [plait.py](https://github.com/plaitpy/plaitpy) | User defined data | From user-defined template with statistical properties | - | [MIT license](https://github.com/plaitpy/plaitpy/blob/master/LICENSE.txt) | Inactive | 400+ |
| [pydbgen](https://github.com/tirthajyoti/pydbgen) | SQL databases and DataFrames  with private information | ease of use | - | MIT | Inactive | 200+ |
| [Synthdet](https://github.com/Unity-Technologies/SynthDet) | Images for object detection  | - | [Article](https://blogs.unity3d.com/2020/09/17/training-a-performant-object-detection-ml-model-on-synthetic-data-using-unity-computer-vision-tools/) | Apache v2.0  | Active | 200+ | 
| [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_regression.html#sklearn.datasets.make_regression) | Random matrices |  -  | - | BSD-3-Clause | Active | 50K+  |
| [timeseries-generator](https://github.com/Nike-Inc/timeseries-generator) | Time-series | GUI, built-in economics factors | - | Apache 2.0 | Active | 60+  |
| [zpy](https://github.com/ZumoLabs/zpy) | Images for machine learning applications| Uses blender to generate images | - | [GPL-v3](https://github.com/ZumoLabs/zpy/blob/main/LICENSE) | Inactive | 200+ |

## Specific use-cases

These packages have more specific use-cases and are not purely generative (listed alphabetically.

| Name | Data type | Extra features | Maintenance | GitHub stars | References | License |
|--|--|--|--|--|--|--|
| [augraphy](https://github.com/sparkfish/augraphy) | Paper documents | - | Active | 50+ | - | MIT |
| [doppelGANger](https://github.com/fjxmlzn/DoppelGANger) | Timeseries generation | Use GANs, high customization | Active | 100+ | [paper](https://arxiv.org/abs/1909.13403) | [BSD-3-Clause-Clear](https://github.com/fjxmlzn/DoppelGANger/blob/master/LICENSE) |
| [mtt-distilation](https://github.com/GeorgeCazenavette/mtt-distillation) | Images for Machine Learning | Distillation from bigger to smaller dataset | Active | 100+ | [paper](https://georgecazenavette.github.io/mtt-distillation/) | MIT
| [smogn](https://github.com/nickkunz/smogn) | Improved tabular dataset | Synthetic Minority Over-Sampling, Pure Python | Active | 100+ | [paper](http://proceedings.mlr.press/v74/branco17a/branco17a.pdf) | GPL-v3 |
| [syndata-generation](https://github.com/debidatta/syndata-generation) | Images for object detection | - | Inactive | 200+ | [paper](https://arxiv.org/abs/1708.01642) | MIT |
| [tofu](https://github.com/spiros/tofu) | UK Biobank synthetic data | - | Inactive | 30+ | - |  [paper](http://doi.org/10.5281/zenodo.3634604) | Missing |
