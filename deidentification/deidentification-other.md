# Deidentification Tools - Other

Here you can find tools meant for deidentifying (research) data and/or checking how well the deidentification process went. 
Any R or Python packages will be later moved to their corresponding files. 
For now, it's easier to first start with one file. 
**This file is Very Much Work In Progress!**

**Important note**  
While some of the below tools promise data "anonymisation", it is by no means guaranteed that the dataset resulting from the deidentification process will indeed be anonymous under the GDPR. You can read more about this in the [Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/personal-data-assess.html).

## Tabular data

**[ARX](https://arx.deidentifier.org/anonymization-tool/)**
- [Open source](https://github.com/arx-deidentifier/arx) software to download and run locally on your PC. It also has an API and a software library for developers.
- Maintenance: Active, 511 GitHub stars
- Features:
  - Explore, transform and clean data
  - Data types: tabular (CSV, Excel, Database files)
  - Privacy models: k-anonymity, l-diversity, t-closeness, β-likeness and δ-disclosure, k-Map, δ-presence, differential privacy and the game-theoretic model. So some background knowledge of any of these models is desirable. 
  - Can analyse both the privacy (risks) and utility of the output data and calculates a way to achieve minimal loss of information while satisfying set criteria. 
  - Techniques: generalisation and top and bottom coding.
- How to: [instruction video](https://www.youtube.com/watch?v=N8I-sxmMfqQ)
  - 1. label if variables are insensitive, identifiers or quasi-identifiers
  - 2. create a generalisation hierarchy for all quasi-identifiers
  - 3. set privacy model configuration(s) and apply weights where necessary (for example to generalise certain variables to a lesser extent)
  - 4. explore the solution space and organise transformations
  - 5. run the anonymisation
  - 6. explore the anonymisation outcome and tweak according to utility and risks.

**[Amnesia](https://amnesia.openaire.eu/)**
- [Open source](https://github.com/dTsitsigkos/Amnesia) software from OpenAIRE which you can [test online](https://amnesia.openaire.eu/amnesia/) or [run locally](https://amnesia.openaire.eu/download.html#). It also has a ReST API.
- Maintenance: active, 128 GitHub stars
- Features
  - Data types: relational tables, set collections, and object-relational tables stored as delimited text files. Metadata from DICOM images can also be loaded into Amnesia.
  - Can export Zenodo and Dataverse 
  - Privacy models: k-anonymity and km-anonymity
  - Techniques: generalisation, masking.
- How to: watch [tutorials](https://amnesia.openaire.eu/tutorials.html) or read the [documentation](https://amnesia.openaire.eu/about-documentation.html#).

**[mu-Argus for microdata](https://research.cbs.nl/casc/mu.htm)**
- [Open source](https://github.com/sdcTools/muargus) software from Statistics Netherlands (CBS) which you can run locally to apply Statistical Disclosure Control techniques to microdata.
- Maintenance: active, 6 GitHub stars
- Features:
  - *TODO*
- How to: a User manual is linked on the [website](https://research.cbs.nl/casc/mu.htm), or see the [step-by-step](https://github.com/sdcTools/manuals/blob/master/mu-argus/Step-by-step%20test%20procedure%20%20MuArgus.pdf) and [getting stated](https://github.com/sdcTools/manuals/blob/master/mu-argus/Getting%20started%20with%20Mu%20Argus.pdf) documentation.

**[sdcMicro](https://shiny.rstudio.com/gallery/sdcapp-microdata.html)**
- [Open source](https://github.com/sdcTools/sdcMicro) [R package](https://cran.r-project.org/web/packages/sdcMicro/index.html) and [web app](https://shiny.rstudio.com/gallery/sdcapp-microdata.html) to apply Statistical Disclosure techniques to microdata. Note that the web app can be used locally without an internet connection.
- Maintenance: active, 57 GitHub stars
- Features:
   - Explore, modify and analyse microdata
   - Data type: tabular data (.Rdata, .sav, .sasb7dat, .csv, .txt, .dta)
   - Privacy models: k-anonymity
   - Anonymisation techniques: generlisation, top-bottom coding, recoding
   - Gives information about disclosure risks and information loss.
   - In the web app, R runs in the background and you can download the underlying R code, making the anonymisation process reproducible.
   - Expoort anonymised data and reports
- How to: check out the [documentation](https://sdctools.github.io/sdcMicro/articles/sdcMicro.html) or watch [this demo](https://youtu.be/JeJ6OOxXZwo?t=5602)

**[Datacheck](https://libscie.github.io/datacheck-website/)**
- Open source [R package](https://libscie.github.io/datacheck/index.html) and a (more limited) web app that checks for presence of common identifiers in tabular datasets. Note that the web app can currently only run in Chrome and Edge browsers as the app is run locally.
- Maintenance: active, 3 GitHub stars, although not published on CRAN yet.
- Features:
  - Data type: tabular data (csv files)
  - R package can check entire folders instead of 1 file at a time.
  - Checks for the following identifiers: Email Address, IPv4, IPv6, MAC Address, Phone Number, Browser User Agent, Latitude Longitude (location), Gender (marginalized groups only, e.g., nonbinary, trans), Social security number, Birthday, Blood Type, IBAN Bank account, Creditcard, Amazon MTurk ID
  - Important note: neither names or indirect identifiers are detected. So even if the web app says a datafile is "safe to share", it may not be! 
- How to: [project report and demo](https://www.youtube.com/watch?v=i5Pa3Sx3n14)


## Qualitative data
**Stanford Named Entity Recognizer**
- *TODO*: Find link and look at features

**[Microsoft Word plugin for labelling text](https://bitbucket.org/ukda/ukds.tools.textanonhelper/wiki/Home)**
- Microsoft Word plugin for labelling numbers and words starting with capital letters in text. These can often be sensitive, for example names, birth dates and addresses.
- [Download here](http://data-archive.ac.uk/media/504356/md5_94fc0c2a25f3a75396059826a23b8224_textanonymisationhelpertool_01_00.zip)
- *TODO*: look at features, provide description 

Acrobat Pro Redac for removing sensitive images and text
- *TODO*: Find open source alternative

**[Masked Piper](https://github.com/WimPouw/TowardsMultimodalOpenScience)**
- Open source tool for masking video data
- [Journal article](https://doi.org/10.1016/j.softx.2022.101236)

**[Textwash](https://github.com/maximilianmozes/textwash)**
- An open source text anonymisation tool based on machine learning
- Currently only available in English, but an interface for Dutch text anonymisation is in the making in the [FAMTAFOS project](https://www.nwo.nl/en/projects/203001143).

Audacity: sound distortion
- *TODO*: provide more information or find open source alternatives

## Neuroimaging data
- Pydeface
- mri_deface
- DeID
- MITRE Identification Scrubber Toolkit
- See also the [Brain MRI Data Sharing Guide](https://doi.org/10.5281/zenodo.3822289)

Techniques: skull stripping, defacing, face blurring, face substitution, see [Eke et al., 2021](https://doi.org/10.1016/j.ynirp.2021.100053). For MEG data, see [Vinding & Oostenveld, 2022](https://doi.org/10.1016/j.neuroimage.2022.119165).

## Other and TODO
Others to check out:
- [OpenPseudonymiser](https://www.openpseudonymiser.org/Default.aspx): Hashing software
- Scrubber
- OpenDP: https://opendp.org/ and https://github.com/opendp/opendp 

