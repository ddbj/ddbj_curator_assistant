# DDBJ Curators' Assistant

The system consists of:
- A set of tools designed to automate and standardize, in a fast and easy way, the curation of Sequence Datasets submitted to DDBJ. It comprises four steps: validation (ddbj_mss_validation); auto-correction (ddbj_autofix); auto upload files to DDBJ Databases (ddbj_sakura2DB); and update work tracking spreadsheet (ddbj_kaeru, "kaeru 帰る" means "leave, go home" in Japanese language, in the sense that the work is done). 
- A database, named dblink_ddbj, that contains the most relevant information from DDBJ Database, designed specially for DDBJ curators.
- An easy-to-use search engine tool, search_dblink, for quickly and simultaneously retrieving data from a wide range of accession IDs.
 
---
## Mass Dataset Documentation

![ag_packages_202204_MSS_workflow](https://github.com/ddbj/ddbj_curator_assistant/assets/85154564/4abd8688-e6bd-40b2-b5c8-90fb59d14032)

Notice ! The MSS tool repository have been migrated to [ddbj/mssassist](https://github.com/ddbj/mssassist).

1. [DDBJ Mass Validation](https://github.com/ddbj/ddbj_curator_assistant/tree/main/ddbj_mss_validation)
   - An easy command line that identifies submitted files (annotation and fasta) and checks inconsistencies based on DDBJ rules.
   - Requirement: BioSample
   - Command line
   ```
   /home/w3const/mssassist/ddbj_mss_validation
   ```
   - Former command line (production)
   ```
   bash /home/andrea/scripts/ddbj_mss_validation
   ```
        - Beta version
        ```
        bash /home/andrea/scripts/ddbj_mss_validation_beta
        ```
3. [DDBJ Autofix](https://github.com/ddbj/ddbj_curator_assistant/tree/main/ddbj_autofix)
   - A simple command line that interactively suggests corrections that have been detected by DDBJ Mss Validation and automatically fixes them.
   - Command line
   ```
   /home/w3const/mssassist/ddbj_autofix
   ```
   - Former command line
   ```
   bash /home/andrea/scripts/ddbj_autofix
   ```
     - Beta (CAUTION! Use this version when running ddbj_mss_validation_beta)
     ```
     bash /home/andrea/scripts/ddbj_autofix_beta
     ```
5. [DDBJ Sakura2DB](https://github.com/ddbj/ddbj_curator_assistant/ddbj_sakura2DB) 
   - Interactive command line that automatically: a) identifies the file type; b) runs sakura2db (test and actual) for the corrected files to upload the files to their respective databases at DDBJ (Tsunami); c) moves the files to DONE directory.
   - Command line
   ```
   /home/w3const/mssassist/ddbj_sakura2DB
   ```
   - Former command line
   ```
   bash /home/andrea/scripts/ddbj_sakura2DB
   ```
      - Beta version
       -  next
     ```
     bash /home/andrea/scripts/ddbj_sakura2DB_beta
     ```
6. [DDBJ Kaeru](https://github.com/ddbj/ddbj_curator_assistant/tree/main/ddbj_kaeru)
   - Update work tracking spreadsheet, after running DDBJ Sakura2DB.
   - Command line
   ```
   /home/w3const/mssassist/ddbj_kaeru
   ```
     - Former command line
     ```
     bash /home/andrea/scripts/ddbj_kaeru
     ```
---
## DBLink DDBJ and Search DBLink Documentation

1. [DBLink DDBJ](https://github.com/ddbj/ddbj_curator_assistant/tree/main/dblink_ddbj)
   - Comprises essential data (dblink dataset) from the major DDBJ databases: BioProject, BioSample, Sequence Read Archive (DRA), Assembled Sequences (Mass Data) and GEA.
2. [Search DBLINK](https://github.com/ddbj/ddbj_curator_assistant/tree/main/search_dblink)
   - A simple command line tool that accesses the DBLink-DDBJ database and correlates the major DBLink dataset from DDBJ using one file with different accession IDs.

