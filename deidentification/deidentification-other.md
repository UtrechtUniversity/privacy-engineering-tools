
# Deidentification Tools - Other

Here you can find tools meant for deidentifying (research) data and/or checking how well the deidentification process went, which do not require any programming experience in R or Python.
Please note that **this file is a Work In Progress!**. Edits will be made, and suggestions for improvement are of course welcome!

**Important note** 
While some of the below tools promise data "anonymization", it is by no means guaranteed that the dataset resulting from the deidentification process will indeed be anonymous under the GDPR. 
You can read more about this in the [Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/personal-data-assess.html).

## Tabular data

| Name | Description | Data type | Privacy models | Other features | Maintenance | GitHub stars | More info | License |
|---|---|---|---|---|---|---|---|---|
| [ARX](https://arx.deidentifier.org/anonymization-tool/) | [Open source](https://github.com/arx-deidentifier/arx) software to anonymize data locally on your PC by generalizing and top- and bottom-coding tabular data.| Tabular (CSV, Excel, Database files) | k-anonymity, l-diversity, t-closeness, β-likeness, δ-disclosure, k-Map, δ-presence, differential privacy, game-theoretic model | Analyze privacy risks and utility of output data, optimizing loss while satisfying set criteria. Has an API and software library. | Active | 500-1000 | [Instruction video](https://www.youtube.com/watch?v=N8I-sxmMfqQ) | [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) |
| [Amnesia](https://amnesia.openaire.eu/) | [Open source](https://github.com/dTsitsigkos/Amnesia) software from OpenAIRE to anonymize data locally on your PC by generalizing and masking tabular data.  | Relational tables, set collections, and object-relational tables stored as delimited text files, metadata from DICOM images. | k-anonymity and km-anonymity | Can export to Zenodo and Dataverse. | Active | 100-500 | [Online demo](https://amnesia.openaire.eu/amnesia/), [tutorials](https://amnesia.openaire.eu/tutorials.html), [documentation](https://amnesia.openaire.eu/about-documentation.html#) | [BSD-3 Clause](https://github.com/dTsitsigkos/Amnesia/blob/master/LICENSE) |
| [sdcMicro](https://shiny.rstudio.com/gallery/sdcapp-microdata.html) | [Open source](https://github.com/sdcTools/sdcMicro) [R package](https://cran.r-project.org/web/packages/sdcMicro/index.html) and [web app](https://shiny.rstudio.com/gallery/sdcapp-microdata.html) to apply Statistical Disclosure techniques such as generalization, top- and bottom coding and recoding to microdata. Web app can run locally. | Tabular data (.Rdata, .sav, .sasb7dat, .csv, .txt, .dta) | k-anonymity | Allows to explore, modify and analyse microdata, gives information about disclosure risks and information loss. Anonymization process of web app can be reproduced. | Active | 10-100 | [Documentation](https://sdctools.github.io/sdcMicro/articles/sdcMicro.html), [demo](https://youtu.be/JeJ6OOxXZwo?t=5602) | [GPL-v2](https://www.r-project.org/Licenses/GPL-2) |
| [mu-Argus](https://research.cbs.nl/casc/mu.htm) | [Open source](https://github.com/sdcTools/muargus) software from Statistics Netherlands (CBS) which you can run locally to apply Statistical Disclosure Control techniques to microdata. | *TBD* | *TBD* | *TBD* | Active | 0-10 | [User manual](https://research.cbs.nl/casc/mu.htm), [step-by-step](https://github.com/sdcTools/manuals/blob/master/mu-argus/Step-by-step%20test%20procedure%20%20MuArgus.pdf), [getting started](https://github.com/sdcTools/manuals/blob/master/mu-argus/Getting%20started%20with%20Mu%20Argus.pdf) | [EUPL-1.2](https://github.com/sdcTools/muargus/blob/master/LICENSE) |
| [Datacheck](https://libscie.github.io/datacheck-website/) | [Open source](https://github.com/libscie/datacheck) [R package](https://libscie.github.io/datacheck/index.html) (not on CRAN yet) and web app that checks for presence of common identifiers in tabular datasets. Web app is Chrome and Edge browsers only. | Tabular data (CSV) | - | Checks for identifiers in a dataset such as email, IP addresses. The R package can check entire folders instead of 1 file at a time. | Active | 0-10 | [Project report and demo](https://www.youtube.com/watch?v=i5Pa3Sx3n14) | [MIT](https://libscie.github.io/datacheck/LICENSE.html) |
| [OpenPseudonymiser](https://www.openpseudonymiser.org/Default.aspx) | Hashing software that replaces identifiers with a "digest", which can be used to link records without disclosing the identifier. | Tabular  (CSV) | Hashing with SHA-2 (256) | Possible to create a salt so that the pseudonymization is a one-way process. You need to register in order to install the software. | Inactive | NA | [Documentation](https://www.openpseudonymiser.org/OpenPseudonymiser_Docs.aspx) | [GPL-v3](https://www.gnu.org/licenses/) |
| [OpenDP](https://opendp.org/) | [Open source](https://github.com/opendp/opendp) libraries for creating differentially private algorithms  | *TODO* | *TODO* | *TODO* | *TODO* | *TODO* | *TODO* | *TODO* |

## Additional notes on packages

#### ARX

When using ARX, you need to label variables as insensitive, identifiers or quasi-identifiers, create generalization hierarchies and set privacy model configurations. Some background knowledge on the available options is therefore required. 

#### OpenAire

While slightly simpler than ARX, some background knowledge on the underlying privacy models is still required.

#### Datacheck

Can detect the following features: Email Address, IPv4, IPv6, MAC Address, Phone Number, Browser User Agent, Latitude Longitude (location), Gender (marginalized groups only, e.g., nonbinary, trans), Social security number, Birthday, Blood Type, IBAN Bank account, Creditcard, Amazon MTurk ID. **Important note**: neither names or indirect identifiers are detected. So even if the web app says a datafile is "safe to share", it may not be!

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

