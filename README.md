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

Then, in both scripts modify the current dictonay for matching the folder name with the `tumor_type` string expected by SigMA, and similarly for the subfolder name with the `data_type` expected by SigMA.

## Intermediate files generated
The R script will generate a folder `Output_SigMA_Rversion` in this the same structure of folders as in the input will be generated. For the python notebook, similarly a folder `Output_SigMA_Py` will be generated. Then, the python notebook will compare the results in `Output_SigMA_Rversion` and `Output_SigMA_Py`.

The main intermediate inputs are the SBS mutational counts in three base context (96 column matrix) and the output from `SigMA::run()`

## Results of comparision

See inside the Python notebook `Comparing_SigMApy_vs_SigMAR.ipynb` to check the results of the comparisions. By now the comparisions are for the columns `sigs_all` and `exps_all`.


