


# Python packages for synthetic data

This is a list of python packages that deal with generating synthetic data. It is compiled mainly through searching in google and GitHub. Naturally, some packages will be missed, so feel free to suggest other packages and make a pull request.

The python packages are subdivided into three different categories: tabular, purely generative and other. This is a loose classification, since packages might fall into multiple categories.

Active maintenance is loosely defined as there being substantial (more than just editing the README) changes to the package in the last year.

## Tabular datasets

This packages in this category are useful if you have a tabular dataset and want to create a new synthetic dataset with similar properties.


| Name | Methods |  Extra Features | Synthetic spectrum | Maintenance | GitHub stars | Paper | License |
|--|--|--|--|--|--|--|--|
| [SDV](https://github.com/sdv-dev/SDV) | Copula, GAN, TVAE | Single table, relational database, time-series, deidentification | synthetically-augmented replica | Active | 900+ | [paper](https://dai.lids.mit.edu/wp-content/uploads/2018/03/SDV.pdf) | MIT | 
| [ydata-synthetic](https://github.com/ydataai/ydata-synthetic) | GAN | Single table and time-series | Synthetically-augmented multivariate plausible | Active | 600+ | - | [MIT license](https://github.com/ydataai/ydata-synthetic/blob/dev/LICENSE) |
| [Gretel Synthetics](https://github.com/gretelai/gretel-synthetics) | LSTM | Differential Privacy | Synthetically-augmented multivariate plausible | Active | 200+ | - | [Apache-2.0 license](https://github.com/gretelai/gretel-synthetics/blob/master/LICENSE) |
| [DataSynthesizer](https://github.com/DataResponsibly/DataSynthesizer) | Bayesian Network | Web User Interface, intermediate file, differential privacy | synthetic structural, synthetically-augmented plausible, synthetically-augmented multivariate plausible | Active | 100+ | [paper](https://github.com/DataResponsibly/DataSynthesizer/blob/master/docs/cr-datasynthesizer-privacy.pdf) | MIT |
| [synthia](https://github.com/dmey/synthia) | fPCA, Gaussian copula, vine copula | Supports xarray | Synthetically-augmented multivariate/univariate plausible| Active | 20+ | [software](https://doi.org/10.21105/joss.02863), [application](https://doi.org/10.5194/gmd-14-5205-2021) | MIT |


## Generative

Generative methods generally do not need any input dataset. Instead the user specifies the properties of the dataset and the package generates the synthetic data from this specification.

| Name | Creates | Extra features | Maintenance | GitHub stars | paper | License |
|--|--|--|--|--|--|--|
| [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_regression.html#sklearn.datasets.make_regression) | Random matrices | - | Active | 50K+ | - | BSD-3-Clause |
| [faker](https://github.com/joke2k/faker) | Many kinds of private information | Modular structure | Active | 10K+ | - | MIT |
| [mimesis](https://github.com/lk-geimfari/mimesis) | Many kinds of private information | High performance, multilingual | Active | 3k+ | - | MIT |
| [BlenderProc](https://github.com/DLR-RM/BlenderProc) | Images for segmentation, distance estimation  |  Physics simulation, camera sampling | Active | 1K+ | [paper](https://arxiv.org/abs/1911.01911) | GPL-v3 |
| [plait.py](https://github.com/plaitpy/plaitpy) | User defined data | From user-defined template with statistical properties | Inactive | 400+ | - | [MIT license](https://github.com/plaitpy/plaitpy/blob/master/LICENSE.txt) |
| [Synthdet](https://github.com/Unity-Technologies/SynthDet) | Images for object detection | - | Active | 200+ | [paper](https://blogs.unity3d.com/2020/09/17/training-a-performant-object-detection-ml-model-on-synthetic-data-using-unity-computer-vision-tools/) | Apache v2.0|
| [pydbgen](https://github.com/tirthajyoti/pydbgen) | SQL databases and DataFrames  with private information | ease of use | Inactive | 200+ | - | MIT |
| [timeseries-generator](https://github.com/Nike-Inc/timeseries-generator) | Time-series | GUI, built-in economics factors | Active | 60+ | - | Apache 2.0 |
| [physim-dataset-generator](https://github.com/cmitash/physim-dataset-generator) | Images for object detection | 3D rendering | Inactive | 60+ | [paper](https://arxiv.org/pdf/1703.03347.pdf) | [BSD-2-Clause license](https://github.com/cmitash/physim-dataset-generator/blob/master/LICENSE) |
| [google-semantic-location-history](https://github.com/UtrechtUniversity/google-semantic-location-history) | Google semantic location histories | - | Active | 2 | - | MIT |


## Specific use-cases

These packages have more specific use-cases and are not purely generative.

| name | Creates | Extra features | Maintenance | GitHub stars | paper | License |
|--|--|--|--|--|--|--|
| [syndata-generation](https://github.com/debidatta/syndata-generation) | Images for object detection | - | Inactive | 200+ | [paper](https://arxiv.org/abs/1708.01642) | MIT |
| [smogn](https://github.com/nickkunz/smogn) | Improved tabular dataset | Synthetic Minority Over-Sampling, Pure Python | Active | 100+ | [paper](http://proceedings.mlr.press/v74/branco17a/branco17a.pdf) | GPL v3 |
| [mtt-distilation](https://github.com/GeorgeCazenavette/mtt-distillation) | Images for Machine Learning | Distillation from bigger to smaller dataset | Active | 100+ | [paper](https://georgecazenavette.github.io/mtt-distillation/) | MIT
| [doppelGANger](https://github.com/fjxmlzn/DoppelGANger) | Timeseries generation | Use GANs, high customization | Active | 100+ | [paper](https://arxiv.org/abs/1909.13403) | [BSD-3-Clause-Clear license](https://github.com/fjxmlzn/DoppelGANger/blob/master/LICENSE) |
| [augraphy](https://github.com/sparkfish/augraphy) | Paper documents | - | Active | 50+ | - | MIT |
| [tofu](https://github.com/spiros/tofu) | UK Biobank synthetic data | - | Inactive | 30+ | - |  [paper](http://doi.org/10.5281/zenodo.3634604) | No License |

