## De-identification tools

The General Data Protection Regulation (GDPR) distinguishes between pseudonymization and anonymization. The goal of both processes is to make data less identifiable, the difference being that anonymization results in data that are no longer subject to the GDPR, whereas pseudonymization results in less identifiable but still personal data. To avoid confusion, we use the term de-identification for the tools listed here, as the goal of these tools is to make data less identifiable, but the result of that process can either consist of pseudonymized or anonymized data.

De-identification can consist of completely removing identifiable information, generalizing data points (e.g., replace birth date with age), replacing identifiable values with non-sensitive ones, etc.
For a comprehensive overview of what de-identification is and how it can be applied to research data, please refer to the [Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/pseudonymisation-anonymisation.html).

We have divided the de-identification tools into three major groups:

1. De-identification tools for which [no programming](deidentification/deidentification-other.md) is required (e.g., complete software packages or graphical user interfaces);
2. [Python packages](deidentification/deidentification-python.md) to de-identify data;
3. [R packages](deidentification-r.md) to de-identify data.

### Currently included tools

The following tools are currently included in this folder:

- Tabular data: 
  - User interfaces: Amnesia, ARX, Datacheck, mu-Argus, OpenPseudonymiser, sdcMicro, tau-Argus
  - Python packages: anonymoUUs, mysto, pynonymizer
  - R packages: Datacheck, sdcMicro, sdcTable
- Textual data: 
  - User interfaces: Stanford Named Entity Recognizer, Text Anonymization Helper
  - Python packages: anonymoUUs, deduce, presidio, Textwash
  - R packages: -
- Images/video: 
  - User interfaces: -
  - Python packages: DeepPrivacy2, Masked-Piper, presidio
  - R packages: -

### Other types of data

Tools for de-identifying the following data types are currently not included:

- **Audio data**: You can de-identify audio data by distorting or otherwise editing the audio track. There are many audio editing tools available, e.g., like the [privacy-friendly tools listed here](https://github.com/CKs-Technology-News/PrivacyTools/blob/main/Desktop%20Tools.md#audio-editing).
- **File metadata**: Many files contain metadata, such as date of creation, instrument settings used, location, etc. These metadata could also be removed if they could reveal personal information. Here is a [list of such metadata removal tools](https://github.com/CKs-Technology-News/PrivacyTools/blob/main/Desktop%20Tools.md#metadata-removal).
- **Neuroimaging data**: Neuroimaging data can be de-identified through skull stripping, defacing, face blurring, and face substitution ([Eke et al., 2021](https://doi.org/10.1016/j.ynirp.2021.100053)). There are many tools available for this (many Python-based), see [this list](https://open-brain-consent.readthedocs.io/en/latest/anon_tools.html) compiled by the Open Brain Consent working group.
- **Databases** (SQL data): There are many tools to de-identify SQL data. However, since this type of data is not often collected as part of the research data (mostly for storing contact details of participants), they are not included in these overviews.

### Other resources

- There is a GitHub organization dedicated to tools to perform [Statistical Disclosure Control](https://github.com/sdcTools). They offer [support](https://github.com/sdcTools/UserSupport) and [documentation](https://github.com/sdcTools/manuals) for sdcMicro, sdcTable, mu-Argus and tau-Argus, among others.
- If you want to know more about Statistical Disclosure Control, the book "[Statistical Disclosure Control](https://doi.org/10.1002/9781118348239)" (Hundepool et al., 2012) gives an extensive overview.
