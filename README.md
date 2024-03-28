# esKnow
This repository contains data and analysis code used in paper: 
Sasmita &amp; Swallow (under review).

# Directory 

Folder: data
>Contains formatted data used for analyses
>>esKnow[1/2]_segmentData.txt - segmentation data organized as each participants' button press times
>>esKnow[1/2]_agreementIndex.txt - agreement index values per participant
>> 
  

Folder: code
>Contains all the codes used for statistical analyses and plotting figures
>>'get.agreement.metrices.R' - contain all the functions to calculate the various agreement measures
>>
>>'esKnow_ManuscriptAnalysis.rmd' - 
>>
>>'esMethods_ManuscriptAnalysis.rmd' - perform all analyses and plotting included in the manuscript, plot output goes to ../plots
>>'esMethods_getFullSampleAgreement.rmd' - calculate the agreement values for the full samples (commercial-lab and everyday-online) used for analyses. This script can act as an example on how to use the functions in get.esMethods.metrics.R
>>
>>'esMethods_getBootstrapStatistics.rmd' - calculate the descriptive statistics (mean of sample means, sd of sample means, sd of population mean, 2.5 & 97.5 percentile of sample means) of bootstrapped agreement values for all sample sizes (n = 2 to 32). Output: .csv files for each agreement measure in each dataset, generated output goes to ../data/summary_statistics

# Run code 

To run all data processing and analyses reported in the manuscript: 
1. Generate bootstrapped data: run 'esMethods_GenerateIterations.rmd'
2. Run analyses and generate plots: run 'esMethods_ManuscriptAnalysis.rmd'
3. Calculate agreement values for the full samples: run 'esMethods_getFullSampleAgreement.rmd'
4. Calculate descriptive statistics for the bootstrapped agreement values: run 'esMethods_getBootstrapStatistics.rmd'
