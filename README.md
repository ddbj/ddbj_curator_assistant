# ddbj_mss_validation

Description
---
Find server hostname and change directory accordingly. In the case of supercom it loads R module and runs jParser and transChecker.
Manages the scripts:

1. [format_files](https://github.com/ddbj/annotator/tree/master/aghelfi/format_files)
2. [mss_validation](https://github.com/ddbj/annotator/tree/master/aghelfi/mss_validation)
3. [common_check](https://github.com/ddbj/annotator/tree/master/aghelfi/common_check)
4. [svp](https://github.com/ddbj/annotator/tree/master/aghelfi/sequence_validator_prototype)
5. [ag_jParser_transChecker](https://github.com/ddbj/annotator/tree/master/aghelfi/nkf_jParser_transChecker)
6. [check output jParser_transChecker](https://github.com/ddbj/annotator/tree/master/aghelfi/nkf_jParser_transChecker)

Usage
---

```
# supercom
bash /home/andrea/scripts/ddbj_mss_validation
```

Output files (Rfixed directory)
---
- mss_validation<br>
confirmation_report.tsv<br>
- svp<br>
warnings_SVP.tsv <br>
- log files <br>
mss_validation.log <br>
svp.log <br>
jParser_transChecker.log<br>

Update
---
<pre>
2023.02.13. released ddbj_mss_validation_sing_v2.1
            Fixed bug on rule_gtag.
2022.04.20. released ddbj_mss_validation_svp_v1.2.sh
            Fixed bug on directory Rfixed for the scripts, common_check_v0.4 and ddbj_filetype_v0.6.
2022.04.18. updated ddbj_mss_validation_svp_v1.1.sh 
            Implements rule CMC0300 on common_check_v0.3
2022.04.13. updated ddbj_mss_validation_svp_v1.0.sh 
            Implements automatic prediction of sub_strain, var, biovar, variety, subtype, cultivar, strain, serovar and chemovar, independent of NCBI taxonomy dump file.
2022.04.12. updated ddbj_mss_validation_svp_v0.9.sh -> ddbj_mss_validation
            Implements common_check_v0.2
2022.04.07. updated ddbj_mss_validation_svp_v0.8.sh
            Implements common_check_v0.1, svp_v1.6, mss_validation_v1.1, formatlinux_remove-blankspaces_v0.4.
2022.03.30. released ddbj_mss_validation_svp_v0.8.sh
            Implements svp_v1.5 (contact, email, ab_name, taxonomy from NCBI private dump file) -> ddbj_mss_validation_beta.
2022.03.23. released ddbj_mss_validation_svp_v0.7.sh
            Sincronizing functions. Changing ANN file directory after run formatlinux_remove-blankspaces.
2022.03.08. released ddbj_mss_validation_svp_v0.6.sh
            The function "formatlinux" is called directly and removed from mss_validation; and the function check_output_jParser_transChecker is waiting ag_jParser_transChecker to finish.
2021.12.24. released ddbj_mss_validation_svp_v0.4.sh
            Show a message on terminal screen if there are errors/warnings on the output of jParser/transChecker.
2021.12.24. released ddbj_mss_validation_svp_v0.3.sh
            Change permission and group owner in all generate dir/files including all ann and fasta files.
2021.12.23. released ddbj_mss_validation_svp_v0.2.sh
            Manages mss_validation and svp. Creates log output files for messages written on terminal.
</pre>
