## Synthetic data

Synthetic data can be a great way make your data less identifiable. It works by creating a new dataset with new people that are not 1 on 1 related to people in the real dataset, thus delivering a level of anonimity, while retaining some (statistical) properties of the original dataset. For a more detailed overview and some of the possible pitfalls of these types of methods, see the [Synthetic data section in the Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/synthetic-data.html).

We have categorized the synthetic data tools in three categories: 

- [R packages](synthetic-simulated-data/synthetic-simulated-r.md);
- [Python packages](synthetic-simulated-data/synthetic-simulated-python.md);
- [Other synthetic data solutions](synthetic-simulated-data/synthetic-simulated-other.md), including some commercial solutions to produce synthetic data.

### Synthetic data vs. simulated data

There is a large number of packages that can *simulate* data. While closely related to synthetic data, we explicitly exclude simulation packages, because of the different aim: usually the aim of simulations is to test hypotheses and validate models, whereas the aim of synthetic data as we use it in this repository is to provide a degree of data protection for real individuals in real datasets.
