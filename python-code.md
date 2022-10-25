# Python code snippets

## [SDV](https://sdv.dev/SDV/index.html)

### [Install](https://sdv.dev/SDV/getting_started/install.html)

```sh
pip install sdv
```
### [Data generation](https://sdv.dev/SDV/user_guides/single_table/tabular_preset.html#tabular-preset)

```python
from sdv.lite import TabularPreset
model = TabularPreset(name="FAST_ML")
model.fit(dataframe)
synthetic_data = model.sample(num_rows=100)
```

## [ydata-synthetic](https://github.com/ydataai/ydata-synthetic)

### Install

```sh
pip install ydata-synthetic
```

### [Data generation](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/gan_example.ipynb)

## [DataSynthesizer](https://github.com/DataResponsibly/DataSynthesizer)

### Install

```sh
pip install DataSyntesizer
```


### [Data generation](https://github.com/DataResponsibly/DataSynthesizer/blob/master/notebooks/DataSynthesizer__correlated_attribute_mode.ipynb)

### Synthia

### [Install](https://dmey.github.io/synthia/installation.html)

```sh
pip install synthia
```
### [Data generation](https://dmey.github.io/synthia/examples/multivariate-gaussian.html)


```python
import synthia as syn
# data is an xarray
generator = syn.CopulaDataGenerator()
parameterizer = syn.QuantileParameterizer(n_quantiles=100)
generator.fit(data, copula=syn.GaussianCopula(), parameterize_by=parameterizer)
samples = generator.generate(n_samples=N_SAMPLES, uniformization_ratio=0, stretch_factor=2)
```

 
