### CMS Data Load and Integrity Tests
This project contains a basic DBT model for loading and exploring CMS data. It includes publically available sample data from CMS, a DBT install to load the data into a database with configuration for datatypes and metadata, and validations to ensure that the data is valid.

Data tests check that the data types are correct and in conventions that match the namespace conventions, for instance:

- NPIs are 10 digit numeric and pass the NPI digit check algorithm: https://www.cms.gov/Regulations-and-Guidance/Administrative-Simplification/NationalProvIdentStand/Downloads/NPIcheckdigit.pdf

Currently, this CMS data file is loaded:

https://data.cms.gov/provider-data/dataset/muwa-iene

```
CMS Medicare PSI-90 and component measures - six-digit estimate dataset
This data set includes the Patient Safety and Adverse Events Composite measure (CMS Medicare PSI 90) and the individual CMS Patient Safety Indicators. CMS Medicare PSI 90 is a composite complication measure composed from 10 separate Patient Safety Indicators. The measure provides an overview of hospital-level quality as it relates to a set of potentially preventable hospital-related events associated with harmful outcomes for patients. NOTICE: Data from the 1st and 2nd quarters of 2020 are not being reported due to the impact of the COVID-19 pandemic. For more information, please reference https://qualitynet.cms.gov/files/5fb838aef61c410025a64709?filename=2020-111-IP.pdf.
Last updated: Sep 23, 2021
Released: Oct 27, 2021
```
