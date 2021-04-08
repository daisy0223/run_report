# RUN_REPORT
This python script is used to transfer TOAST's aggregating excel output into a PDF run report.


## Contents for Input Excel

- Sample
- Pangolin
- NextClade
- DB_versions
- Assem_Stat
- VADR Stat
- Assem_Len
- Frac_N
- Depth
- Coverage
- Variants
- VADR_Alrts
- VADR_Info


## Prerequisites
- `python` version >= ~3.0
- `reportlab` 
- `pypdf2` 

## Building


```Shell
$> python3 input.xlxs run_report.pdf
```

