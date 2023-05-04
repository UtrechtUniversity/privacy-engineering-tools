# De-identification Tools - User interfaces

Here you can find tools meant for de-identifying (research) data and/or checking how well the de-identification process went, which do not require any programming experience in R or Python - most of the tools listed below are user interfaces, meaning there is no programming required.

### Important note
Some of the below tools promise data "anonymization", but it is by no means guaranteed that the dataset resulting from the de-identification process will indeed be anonymous under the GDPR. 
You can read more about this in the [Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/personal-data-assess.html).

## Tabular data

Sorted alphabetically, here are the most relevant de-identification tools we found:

| Name | Description | Data type | Privacy models | More info | License | Maintenance | GitHub stars |
|---|---|---|---|---|---|---|---|
| [Amnesia](https://amnesia.openaire.eu/) | Anonymization using generalization and masking, can export to Zenodo and Dataverse | Relational tables, set collections, DICOM metadata | k-anonymity, km-anonymity | [Online demo](https://amnesia.openaire.eu/amnesia/), [tutorials](https://amnesia.openaire.eu/tutorials.html), [documentation](https://amnesia.openaire.eu/about-documentation.html#) | [BSD-3 Clause](https://github.com/dTsitsigkos/Amnesia/blob/master/LICENSE) | Active | 100-500 
| [ARX](https://arx.deidentifier.org/anonymization-tool/) | Anonymization using generalization and top- and bottom-coding + analyze privacy risks and utility | Tabular (CSV, Excel, Database files) | k-anonymity, l-diversity, t-closeness, β-likeness, δ-disclosure, k-Map, δ-presence, differential privacy, game-theoretic model |  [Instruction video](https://www.youtube.com/watch?v=N8I-sxmMfqQ) | [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) | Active | 500-1000 | 
| [Datacheck](https://libscie.github.io/datacheck-website/) | [Open source](https://github.com/libscie/datacheck) [R package](https://libscie.github.io/datacheck/index.html) and web app to check the presence of common identifiers | Tabular data (CSV) | - |  [Project report and demo](https://www.youtube.com/watch?v=i5Pa3Sx3n14) | [MIT](https://libscie.github.io/datacheck/LICENSE.html) | Active | 0-10 |
| [mu-Argus](https://research.cbs.nl/casc/mu.htm) | Statistical Disclosure Control from CBS | microdata (individual-level) | Global recoding, local suppression, top and bottom coding, PRAM. | [User manual](https://research.cbs.nl/casc/mu.htm), [more manuals](https://github.com/sdcTools/manuals/blob/master/mu-argus) | [EUPL-1.2](https://github.com/sdcTools/muargus/blob/master/LICENSE) | Active | 0-10 |
| [OpenPseudonymiser](https://www.openpseudonymiser.org/Default.aspx) | Hashing software (registration required) | Tabular  (CSV) | Hashing (SHA-256) | [Documentation](https://www.openpseudonymiser.org/OpenPseudonymiser_Docs.aspx) | [GPL-v3](https://www.gnu.org/licenses/) |  Inactive | NA |
| [sdcMicro](https://shiny.rstudio.com/gallery/sdcapp-microdata.html) | [R package](https://cran.r-project.org/web/packages/sdcMicro/index.html) and [web app](https://shiny.rstudio.com/gallery/sdcapp-microdata.html) to apply generalization, top- and bottom coding, recoding + analyze privacy risks and utility | Tabular data (.Rdata, .sav, .sasb7dat, .csv, .txt, .dta) | k-anonymity | [Documentation](https://sdctools.github.io/sdcMicro/articles/sdcMicro.html), [demo](https://youtu.be/JeJ6OOxXZwo?t=5602) | [GPL-v2](https://www.r-project.org/Licenses/GPL-2) | Active | 10-100 |
| [tau-Argus](https://research.cbs.nl/casc/tau.htm) | Statistical Disclosure Control from CBS | tables (e.g., frequency tables) | Recoding, suppression (hypercube, modular, network, optimal) | [User manual](https://research.cbs.nl/casc/Software/TauManualV4.1.pdf), [more manuals](https://github.com/sdcTools/manuals/blob/master/tau-argus) | [EUPL-1.2](https://github.com/sdcTools/tauargus/blob/master/LICENSE) | Active | 0-10 

You can find a more detailed comparison between ARX, mu-Argus, sdcMicro and Amnesia in [Stenersen (2020)](https://www.duo.uio.no/bitstream/handle/10852/79902/13/Anonymization-of-Health-Data.pdf#page=75) ([persistent link](http://hdl.handle.net/10852/79902)).

## Textual data

| Name | Description | Data type |  More info | License | Maintenance | GitHub stars |
|---|---|---|---|---|---|---|
| [Stanford Named Entity Recognizer](https://nlp.stanford.edu/software/CRF-NER.html) | Java-based recognition interface of English entities (e.g., Person, Organization, Location)  | Text | - | [GNU-GPL-v2](http://www.gnu.org/licenses/gpl-2.0.html) | Inactive | -
| [Text Anonymization Helper](https://bitbucket.org/ukda/ukds.tools.textanonhelper/wiki/Home) | Microsoft Word plugin for finding and labelling potentially identifiable text | Text | [Download](http://data-archive.ac.uk/media/504356/md5_94fc0c2a25f3a75396059826a23b8224_textanonymisationhelpertool_01_00.zip) | [Custom license](https://bitbucket.org/ukda/ukds.tools.textanonhelper/wiki/LICENSE) | Inactive | -
