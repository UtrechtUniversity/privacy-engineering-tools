

# Deidentification Tools - Other

Here you can find tools meant for deidentifying (research) data and/or checking how well the deidentification process went, which do not require any programming experience in R or Python.
Please note that **this file is a Work In Progress!**. Edits will be made, and suggestions for improvement are of course welcome!

**Important note** 
While some of the below tools promise data "anonymization", it is by no means guaranteed that the dataset resulting from the deidentification process will indeed be anonymous under the GDPR. 
You can read more about this in the [Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/personal-data-assess.html).

## Tabular data

| Name | Description | Data type | Privacy models |  More info | License | Maintenance | GitHub stars |
|---|---|---|---|---|---|---|---|---|
| [ARX](https://arx.deidentifier.org/anonymization-tool/) | Top- and bottom-coding | Tabular (CSV, Excel, Database files) | k-anonymity, l-diversity, t-closeness, β-likeness, δ-disclosure, k-Map, δ-presence, differential privacy, game-theoretic model |  [Instruction video](https://www.youtube.com/watch?v=N8I-sxmMfqQ) | [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) | Active | 500-1000 | 
| [Amnesia](https://amnesia.openaire.eu/) | Generalization and masking of tabular data  | Relational tables, set collections, metadata from DICOM images. | k-anonymity and km-anonymity | [Online demo](https://amnesia.openaire.eu/amnesia/), [tutorials](https://amnesia.openaire.eu/tutorials.html), [documentation](https://amnesia.openaire.eu/about-documentation.html#) | [BSD-3 Clause](https://github.com/dTsitsigkos/Amnesia/blob/master/LICENSE) | Active | 100-500 
| [sdcMicro](https://shiny.rstudio.com/gallery/sdcapp-microdata.html) | [R package](https://cran.r-project.org/web/packages/sdcMicro/index.html) and [web app](https://shiny.rstudio.com/gallery/sdcapp-microdata.html), generalization and top- and bottom coding | Tabular data (.Rdata, .sav, .sasb7dat, .csv, .txt, .dta) | k-anonymity | [Documentation](https://sdctools.github.io/sdcMicro/articles/sdcMicro.html), [demo](https://youtu.be/JeJ6OOxXZwo?t=5602) | [GPL-v2](https://www.r-project.org/Licenses/GPL-2) | Active | 10-100 |
| [mu-Argus](https://research.cbs.nl/casc/mu.htm) | Statistical Disclosure Control from CBS | microdata | Global recoding, local suppression, top and bottom coding, PRAM. | [User manual](https://research.cbs.nl/casc/mu.htm), [step-by-step](https://github.com/sdcTools/manuals/blob/master/mu-argus/Step-by-step%20test%20procedure%20%20MuArgus.pdf), [getting started](https://github.com/sdcTools/manuals/blob/master/mu-argus/Getting%20started%20with%20Mu%20Argus.pdf) | [EUPL-1.2](https://github.com/sdcTools/muargus/blob/master/LICENSE) | Active | 0-10 |
| [Datacheck](https://libscie.github.io/datacheck-website/) | [Open source](https://github.com/libscie/datacheck) [R package](https://libscie.github.io/datacheck/index.html) and web app, presence of common identifiers. | Tabular data (CSV) | - |  [Project report and demo](https://www.youtube.com/watch?v=i5Pa3Sx3n14) | [MIT](https://libscie.github.io/datacheck/LICENSE.html) | Active | 0-10 |
| [OpenPseudonymiser](https://www.openpseudonymiser.org/Default.aspx) | Hashing software, needs registration | Tabular  (CSV) | Hashing | [Documentation](https://www.openpseudonymiser.org/OpenPseudonymiser_Docs.aspx) | [GPL-v3](https://www.gnu.org/licenses/) |  Inactive | NA |
| [OpenDP](https://opendp.org/) | Community of [Open source](https://github.com/opendp/opendp) libraries with differentially private algorithms  | - | Differential Privacy | - | [GitHub](https://github.com/opendp) | Active | - |

## Qualitative data (TODO)

We need to look into tools to deidentify qualitative data a bit more. In the meantime, here are a few first ones:
- **Stanford Named Entity Recognizer**
  - *TODO*: Find link and look at features
- **[Microsoft Word plugin for labelling text](https://bitbucket.org/ukda/ukds.tools.textanonhelper/wiki/Home)**
  - Microsoft Word plugin for labelling numbers and words starting with capital letters in text. These can often be sensitive, for example names, birth dates and addresses.
  - [Download here](http://data-archive.ac.uk/media/504356/md5_94fc0c2a25f3a75396059826a23b8224_textanonymisationhelpertool_01_00.zip)
  - *TODO*: look at features, provide description 
- Acrobat Pro Redac for removing sensitive images and text
  - *TODO*: Find open source alternative
- Audacity: sound distortion
  - *TODO*: provide more information and/or find open source alternatives

## Neuroimaging data
Neuroimaging data can be deidentified through skull stripping, defacing, face blurring, face substitution, see [Eke et al., 2021](https://doi.org/10.1016/j.ynirp.2021.100053). There are many tools available for this, such as Pydeface, mri_deface, DeID, MITRE Identification Scrubber Toolkit, etc. Most of these are python-based tools, so these will have to be transferred to the Python file anyways. For MEG data, please read more in [Vinding & Oostenveld, 2022](https://doi.org/10.1016/j.neuroimage.2022.119165). For general instructions on how to share Brain MRI data, please see the [Brain MRI Data Sharing Guide](https://doi.org/10.5281/zenodo.3822289).

