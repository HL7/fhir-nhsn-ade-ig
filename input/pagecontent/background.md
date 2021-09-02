### Background

Inpatient hypoglycemia is one of the most common adverse drug events (ADEs) occurring in United States (U.S.) hospitals. Hypoglycemia in hospitalized patients can be severe and life-threatening and is associated with longer hospital stays and increased medical costs. Measurement of medication-related hypoglycemia in a meaningful and standardized way could improve hospital glycemic management. The NHSN Adverse Drug Event-Hypoglycemia FHIR implementation guide (IG) seeks to enable EHRs to serve as source systems for reporting linked inpatient blood glucose and medication administration data to the Centers for Disease Control and Prevention (CDC) National Healthcare Safety Network (NHSN) via industry electronic messages, with the goals of improving patient safety and facilitating hospital quality improvement efforts and benchmarking of hypoglycemia.

### Scope

This IG addresses blood glucose and medication administration events in inpatient settings only and does not include hypoglycemia resulting only in outpatient care (e.g., hypoglycemia resulting in emergency medical services, physician office visits, or emergency department visits only). This IG addresses ADE data collection at the patient-level (i.e., collects individual laboratory and point-of-care-blood glucose and individual medication data for each inpatient encounter). The IG does not describe the calculation of any measures for hypoglycemia rates; these measures are intended to be calculated, aggregated, or risk-adjusted subsequent to reporting of patient-level data to CDC.

### Patient-Level Data Calculations

The patient level data recieved will be used by NHSN to calculate:

* What is the rate of hypoglycemic events as defined per the National Quality Forum (NQF) quality measure [#2363](https://cmit.cms.gov/CMIT_public/ViewMeasure?MeasureId=3180)? (The number of inpatient hypoglycemia events preceded by antidiabetic drug / the number of inpatient days with ≥1 antidiabetic drug administered).
* What is the rate of hypoglycemic events as defined per the NQF quality measure [#3503](https://cmit.cms.gov/CMIT_public/ViewMeasure?MeasureId=6086)? (The number of inpatient admissions with hypoglycemia events preceded by antidiabetic drug / the number of inpatient admissions with ≥1 antidiabetic drug administered).
* What percentage of patients with ≥1 antidiabetic drug administered had a recurrent hypoglycemic day or event during their hospital stay?
* What are the hospital’s hypoglycemia rates stratified by critical care vs. non-critical care locations?
* What is the percentage of hospital antidiabetic drug days where blood glucose was < 40 mg/dL, < 54 mg/dL, or < 70 mg/dL?
* How do aggregate hospital hypoglycemia rates differ by hospital type, hospital size, and other variables?

### Relationship to Other Guides/Work

Similar standards that seek to report ADEs include: 
* [Profiles for ICSR Transfusion and Vaccination Adverse Event Detection and Reporting](https://build.fhir.org/ig/HL7/fhir-icsr-ae-reporting/branches/main/index.html).
* [ISO/HL7 27953-2:2011: Health informatics — Individual case safety reports (ICSRs) in pharmacovigilance — Part 2: Human pharmaceutical reporting requirements for ICSR](https://www.iso.org/standard/53825.html)