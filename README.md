# RUN_REPORT
This python script is used to transfer TOAST's aggregating excel output into a PDF run report.


## Contents for Input Excel

- `Sample`: Sample name
- `Pangolin`: Pangolin lineage
- `NextClade`: NextClade clade
- `DB_versions`: Database versions of Pangolin and Nextclade. Format is Pangolin_DB:Nextclade_DB.
- `Assem_Stat`: Pass/Fail. The default thresholds are a sequence length >= 15000 bases and the fraction of N's <= 0.10.
- `VADR Stat`: Pass/Fail. Fail indicates the sequence contained VADR fail alerts.
- `Assem_Len`: Length of the consensus sequence
- `Frac_N`: Percentage of N's in the consensus sequence
- `Depth`: Average read mapping depth
- `Coverage`: Breath of coverage
- `Variants`: Amino acid variants identified. The pipe symbol '|' separates substitutions (left) and deletions (right). Format is Gene:Amino Acid Variant.
- `VADR_Alrts`: VADR alerts identified in the consensus sequence. Multiple alerts are separated by colons.
- `VADR_Info`: If the sample contains one of four alert codes associated with an indel (fsthicnf, deletins, unexleng, insertnp, deletinp, deleting), the program will output the gene and coordinate range of the indel feature. Multiple indel features are separated by semicolons. Format is Gene:Feature-Start:Feature-End. 


## Prerequisites
- `pandas, numpy, csv, datetime, matplotlib, reportlab, textwrap, pypdf2` 

## Usage
```Shell
$> python3 autoreport.py /path/to/input.xlsx /path/to/output.pdf /path/to/toast_logo.png
```

