# DDBJ Curators' Assistant

The system consists of a database, named dblink_ddbj, that contains the most relevant information from DDBJ Database designed specially for DDBJ curators, an easy-to-use search engine tool, search_dblink, for quick data retrieval and a set of tools designed to validate (ddbj_mss_validation), and quickly auto-correct (ddbj_autofix) files submitted to DDBJ's Mass Submission System. Besides, it includes two other tools that automatically upload files to DDBJ Database (ddbj_sakura2DB) and update Google spreadsheet (ddbj_kaeru) for work tracking.  

---
## Mass Dataset Documentation

![ag_packages_202204_MSS_workflow](https://github.com/ddbj/ddbj_curator_assistant/assets/85154564/afb41b5b-da4e-4cf0-9ceb-bca6d9058b91)

1. [DDBJ Mass Validation](https://github.com/ddbj/ddbj_curator_assistant/tree/main/ddbj_mss_validation)
   - An easy command line that identifies submitted files (annotation and fasta) and checks inconsistencies based on DDBJ rules. 
2. [DDBJ Autofix](https://github.com/ddbj/ddbj_curator_assistant/tree/main/ddbj_autofix)
   - A simple command line that automatically fix the errors detected by DDBJ Mss Validation.
3. [DDBJ Sakura2DB](https://github.com/ddbj/ddbj_curator_assistant/ddbj_sakura2DB) 
     - Upload corrected files, annotation and fasta, to Tsunami DB.
4. [DDBJ Kaeru](https://github.com/ddbj/ddbj_curator_assistant/tree/main/ddbj_kaeru)
     - Update work tracking spreadsheet.
---
## DBLink DDBJ and Search DBLink Documentation

1. [DBLink DDBJ](https://github.com/ddbj/ddbj_curator_assistant/tree/main/dblink_ddbj)
   - Comprises essential data (dblink dataset) from the major DDBJ databases: BioProject, BioSample, Sequence Read Archive (DRA), Assembled Sequences (Mass Data) and GEA.
2. [Search DBLINK](https://github.com/ddbj/ddbj_curator_assistant/tree/main/search_dblink)
   - A simple command line tool that accesses the DBLink-DDBJ database and correlates the major DBLink dataset from DDBJ using one file with different accession IDs.

