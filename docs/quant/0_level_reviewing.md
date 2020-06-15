
### MassIVE.quant : Level of integrity or reproducibility

xxx

### MassIVE.quant reviewed - Bronze (Automatic review) : 

1. Check ‘Metadata’ includes the required column headers : Condition, BioReplicate, Run ( or Raw.files)
2. Check whether the raw files in metadata are available in ‘raw spectrum files’ collection or not.
3. Check any files in ‘Quantification’ collection
3. Check any files in ‘Statistical Analysis of Quantified Analytes’ collection

If got ‘Bronze’ level, the dataset would be shown in ‘MassIVE.quant’ table.

###  MassIVE.quant reviewed - Silver (Manual review)
1. Metadata 
    * Summary statistics in the blue box are correct or not.
    * Correctly annotated for biological replicate
    * Correctly reported technical replicate and fraction.
    * More information is optional.

2. Quantification 
    * Feature-level or protein-level quantification is available or not.
    * File can be parsed and showed up for browsing or not. For example, xls file with multiple sheets can not be parsed.

3. Statistical Analysis of Quantified Analytes
    * Check whether it is meaningful information or not.  
    * Files can be parsed and showed up for browsing or not. For example, xls file with multiple sheets can not be parsed.
    * !! Note : it does not need to be the MSstats output format.

###  MassIVE.quant reviewed - Gold (Manual review) : Level 1 + Check repeatability
1. Check parameter files or configuration files are available to repeat the same conclusion in ‘Statistical Analysis of Quantified Analytes’s collection
    * mqpar.xml, parameter files for MaxQuant -> Method collection
    * Log files for MSstats -> Method collection
    * R script or any script is available to reproduce statistical analysis.
    * Tool-specific files including these information as alternatives, such as .pdresult, .pdstudy, .sne, .sky and so on
    * Or other configuration file to repeat the same analysis
    * !! Note : it doesn’t mean to reproduce the same conclusion in the original publication.
    * !! Note : We don’t review or evaluate the method itself.

###  MassIVE.quant reviewed - Platinum (Manual review) : Level 2 + Check reproducibility for publication 
1. The reproduced results were published in a peer-reviewed manuscript.
    * This can be referred for the publication.
    * !! Note : We don’t review or evaluate the method itself.

