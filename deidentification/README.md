## De-identification

The General Data Protection Regulation (GDPR) distinguishes between pseudonymization and anonymization. The goal of both processes is to make data less identifiable, the difference being that anonymization results in data that are no longer subject to the GDPR, whereas pseudonymization results in less identifiable but still personal data. To avoid confusion, we use the term de-identification for the tools listed here, as the goal of these tools is to make data less identifiable, but the result of that process can either consist of pseudonymized or anonymized data.

De-identification can consist of completely removing identifiable information, generalizing data points (e.g., replace birth date with age), replacing identifiable values with non-sensitive ones, etc.
For a comprehensive overview of what de-identification is and how it can be applied to research data, please refer to the [Data Privacy Handbook](https://utrechtuniversity.github.io/dataprivacyhandbook/pseudonymisation-anonymisation.html).

We have divided the de-identification tools into three major groups:

1. De-identification tools for which [no programming](deidentification/deidentification-other.md) is required (e.g., complete software packages or graphical user interfaces);
2. [Python packages](deidentification/deidentification-python.md) to de-identify data;
3. [R packages](deidentification-r.md) to de-identify data.
