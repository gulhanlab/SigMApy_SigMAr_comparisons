# SigMApy_SigMAr_comparisons
Scripts to compare the results from SigMA in R version with the SigMA in Python version

## Description of analysis

The script `SigMA_running_TCGA_groundtruth.Rmd` will run SigMA_R (in R) for all the input folders and files. And then, run the script `Comparing_SigMApy_vs_SigMAR.ipynb` to run the SigMA in python version and compare the results with the SigMA_R. 

## How to set up the input

Create an input dataset folder with the next structure:

```
├── BRCA
│   ├── Foundation_One
│   ├── mc3
│   ├── MSK_IMPACTv1
│   └── MSK_IMPACTv2
├── COADREAD
│   ├── Foundation_One
│   ├── MSK_IMPACTv1
│   └── MSK_IMPACTv2
└── PAAD
    ├── mc3
    └── SeqCap_capture_targets
```
