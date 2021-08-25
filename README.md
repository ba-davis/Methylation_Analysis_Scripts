# Methylation_Analysis_Scripts

Code for analyzing DNA methylation next gen sequencing data.

Typically this is bisulfite converted DNA with C counts and T counts.  
For example: WGBS, RRBS, Methyl-Seq


## Code
### ide_scripts
**general_functions.R** Includes custom functions that do not require methylKit.
Operates on general objects that may be shared across different frameworks.
Currently just a couple of functions for PCA (describe and plot).

**methylkit_framework_ide.R**: Includes custom functions that require methylkit to perform ide on BS seq data.
Uses output of Bismark as input: cytosine reports or coverage files.  
Requires a metadata excel file with sample names and groups/covariates.

### diff_analysis_scripts
**methylkit_diff_functions.R**: functions to perform differential analysis using methylKit framework.
