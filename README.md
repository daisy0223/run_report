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
- `pandas, numpy, csv, datetime, matplotlib, reportlab, texwrap, pypdf2` 

## Usage
```Shell
$> python3 autoreport.py /path/to/input.xlsx /path/to/output.pdf /path/to/toast_logo.png
```

