# Python packages to create synthetic data

This is a list of Python packages that can help you generate synthetic data. The list was compiled mainly through searching in Google and GitHub. Naturally, some packages will be missing, so feel free to suggest other packages.

We divided the packages into three categories: Tabular dataset, Purely generative datasets and packages for specific use cases. This is a loose classification, since packages might fall into multiple categories.

## Tabular datasets

This packages in this category are useful if you have a tabular dataset and want to create a new synthetic dataset with similar properties (listed in alphabetical order).

| Name | Methods |  Extra Features | Synthetic spectrum | More info | License | Maintenance | GitHub stars
|--|--|--|--|--|--|--|--|
| [DataSynthesizer](https://github.com/DataResponsibly/DataSynthesizer) | Bayesian Network | Web User Interface, intermediate file, differential privacy | Synthetic structural, synthetically-augmented plausible, synthetically-augmented multivariate plausible | [Article](https://github.com/DataResponsibly/DataSynthesizer/blob/master/docs/cr-datasynthesizer-privacy.pdf), [on PyPi](https://pypi.org/project/DataSynthesizer/) | [MIT](https://github.com/DataResponsibly/DataSynthesizer/blob/master/LICENSE) | Active | 100-500
| [Gretel Synthetics](https://github.com/gretelai/gretel-synthetics) | LSTM | Differential Privacy | Synthetically-augmented multivariate plausible | [Documentation](https://synthetics.docs.gretel.ai/en/stable/), [on PyPi](https://pypi.org/project/gretel-synthetics/) | [Apache-2.0](https://github.com/gretelai/gretel-synthetics/blob/master/LICENSE) | Active | 100-500
| [MetaSynth](https://github.com/sodascience/metasynth) | Scipy | intermediate file, extensible | Synthetically-augmented univariate plausible | [Documentation](https://metasynth.readthedocs.io/en/latest/index.html), [PyPi](https://pypi.org/project/metasynth/) | [MIT](https://github.com/sodascience/metasynth/blob/main/LICENSE) | Active | 0-10
| [Synthetic Data Vault](https://github.com/sdv-dev/SDV) (SDV) | Copula, GAN, TVAE | Single table, relational database, time-series, de-identification | Synthetically-augmented replica | [Article](https://doi.org/10.1109/DSAA.2016.49) ([pdf](https://dai.lids.mit.edu/wp-content/uploads/2018/03/SDV.pdf)), [documentation](https://docs.sdv.dev/sdv/) | [MIT](https://github.com/sdv-dev/SDV/blob/master/LICENSE) | Active | 500-1000
| [synthia](https://github.com/dmey/synthia) | fPCA, Gaussian copula, vine copula | Supports xarray | Synthetically-augmented multivariate/univariate plausible| [Article](https://doi.org/10.21105/joss.02863), [article](https://doi.org/10.5194/gmd-14-5205-2021), [documentation](https://dmey.github.io/synthia/) | [MIT](https://github.com/dmey/synthia/blob/master/LICENSE.txt) | Active | 10-100
| [ydata-synthetic](https://github.com/ydataai/ydata-synthetic) | GAN | Single table and time-series | Synthetically-augmented multivariate plausible | [On PyPi](https://pypi.org/project/ydata-synthetic/) | [MIT](https://github.com/ydataai/ydata-synthetic/blob/dev/LICENSE) | Active | 500-1000

## Generative

Generative methods generally do not need any input dataset. Instead, the user specifies the properties of the dataset and the package generates the synthetic data from this specification (listed in alphabetical order).

| Name | Data type | Extra features | More info |  License | Maintenance | GitHub stars |
|--|--|--|--|--|--|--|
| [BlenderProc](https://github.com/DLR-RM/BlenderProc) | Images for segmentation, distance estimation  |  Physics simulation, camera sampling | [Article](https://doi.org/10.48550/arXiv.1911.01911), [documentation](https://dlr-rm.github.io/BlenderProc/) | [GPL-v3](https://github.com/DLR-RM/BlenderProc/blob/main/LICENSE) | Active | 1000+ |
| [faker](https://github.com/joke2k/faker) | Many kinds of identifiers, e.g., name, address, phone number, etc. | Modular structure | [Documentation](https://faker.readthedocs.io/en/master/), [on PyPi](https://pypi.org/project/Faker/) | [MIT](https://github.com/joke2k/faker/blob/master/LICENSE.txt) | Active | 1000+
| [google-semantic-location-history](https://github.com/UtrechtUniversity/google-semantic-location-history) | Google semantic location histories | Uses GenSON, Faker, faker-schema | - | [MIT](https://github.com/UtrechtUniversity/google-semantic-location-history/blob/main/LICENSE) | Active | 0-10 |
| [mimesis](https://github.com/lk-geimfari/mimesis) | Many kinds of identifiers, e.g., name, address, phone number, etc. (databases, json, xml) | High performance, multilingual | [Documentation](https://mimesis.name/en/master/), [on PyPi](https://pypi.org/project/mimesis/) | [MIT](https://github.com/lk-geimfari/mimesis/blob/master/LICENSE) | Active | 1000+ |
| [physim-dataset-generator](https://github.com/cmitash/physim-dataset-generator) | Images of cluttered scenes to train object detection models | 3D rendering | [Article](https://doi.org/10.1109/IROS.2017.8202206) | [BSD-2 Clause](https://github.com/cmitash/physim-dataset-generator/blob/master/LICENSE) | Inactive | 10-100 |
| [plait.py](https://github.com/plaitpy/plaitpy) | Tabular data | From user-defined yaml template | - | [MIT](https://github.com/plaitpy/plaitpy/blob/master/LICENSE.txt) | Inactive | 100-500 |
| [pydbgen](https://github.com/tirthajyoti/pydbgen) | SQL databases and DataFrames  with private information | Easy to use, uses Faker | [Documentation](https://pydbgen.readthedocs.io/en/latest/) | [MIT](https://github.com/tirthajyoti/pydbgen/blob/master/LICENSE.txt) | Inactive | 100-500 |
| [Synthdet](https://github.com/Unity-Technologies/SynthDet) | Images to train object detection models | - | [Article](https://blogs.unity3d.com/2020/09/17/training-a-performant-object-detection-ml-model-on-synthetic-data-using-unity-computer-vision-tools/) | [Apache 2.0](https://github.com/Unity-Technologies/SynthDet/blob/master/LICENSE.md)  | Active | 100-500 | 
| [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_regression.html#sklearn.datasets.make_regression) | Random matrices (regression problem) |  -  | - | [BSD-3 Clause](https://github.com/scikit-learn/scikit-learn/blob/main/COPYING) | Active | 1000+  |
| [timeseries-generator](https://github.com/Nike-Inc/timeseries-generator) | Time-series | GUI, built-in economics factors | - | [Apache 2.0](https://github.com/Nike-Inc/timeseries-generator/blob/master/LICENSE) | Active | 10-100  |
| [zpy](https://github.com/ZumoLabs/zpy) | Images for machine learning applications | Uses blender to generate images | - | [GPL-v3](https://github.com/ZumoLabs/zpy/blob/main/LICENSE) | Inactive | 100-500 |

## Specific use-cases

These packages have more specific use-cases and are not purely generative (listed alphabetically).

| Name | Data type | Extra features | More info | License | Maintenance | GitHub stars |
|--|--|--|--|--|--|--|
| [augraphy](https://github.com/sparkfish/augraphy) | Distortion of paper documents | - | - | [MIT](https://github.com/sparkfish/augraphy/blob/dev/LICENSE) | Active | 10-100 |
| [doppelGANger](https://github.com/fjxmlzn/DoppelGANger) | Timeseries generation | Uses GANs, high customization | [Article](https://doi.org/10.48550/arXiv.1909.13403), [presentation](https://doi.org/10.1145/3419394.3423643) | [BSD-3 Clause-Clear](https://github.com/fjxmlzn/DoppelGANger/blob/master/LICENSE) | Active | 100-500 |
| [mtt-distilation](https://github.com/GeorgeCazenavette/mtt-distillation) | Images for Machine Learning | Distillation from bigger to smaller dataset | [Article](https://doi.org/10.48550/arXiv.2203.11932/) | [MIT](https://github.com/GeorgeCazenavette/mtt-distillation/blob/main/LICENSE.txt) | Active | 100-500 | 
| [smogn](https://github.com/nickkunz/smogn) | Improved tabular dataset | Synthetic Minority Over-Sampling, Pure Python | [Article](http://proceedings.mlr.press/v74/branco17a/branco17a.pdf), [on PyPi](https://pypi.org/project/smogn) | GPL-v3 | Active | 100-500 |
| [syndata-generation](https://github.com/debidatta/syndata-generation) | Synthetic images (scenes, bounding box annotations) to train object detection models | - | [Article](https://doi.org/10.48550/arXiv.1708.01642) | [MIT](https://github.com/debidatta/syndata-generation/blob/master/LICENSE) | Inactive | 100-500 |
| [tofu](https://github.com/spiros/tofu) | Synthetic UK Biobank data | - | [Published version](http://doi.org/10.5281/zenodo.3634604) | [MIT](https://choosealicense.com/licenses/mit/) | Inactive | 10-100 |
