# HCC_Detection_Paper
Code for the paper "Machine learning-enabled early detection of hepatocellular carcinoma utilizing cell-free DNA mutation and fragmentation multiplicity: a prospective study"

First download and unzip the PREDICT_Dataset.zip file

Code and dataset deposited in this repository main contained the following parts:
### Key discoveries during the research:
1. The mutation list identified in retrospective cohort:
```
./0_Key_Discoveries/0_Retrospective_Mutations
```

2. The HBV integration event identified in retrospective cohort:
```
./0_Key_Discoveries/1_HBV_Event
```

3. The CNV identified in retrospective cohort by CONTRA and ichorCNA tools:
```
./0_Key_Discoveries/2_Segments_from_ichorCNA
./0_Key_Discoveries/3_Gene_annotations_from_CONTRA
```

### Code for the computing of SNVScore, FRAGScore and IFScore
1. SNVScore:
```
Run ./000_Code_Directory/PREDICT_Code/SNVScore/snv_model.py, using input "SNV_features_retrospective.xlsx"
```

2. FRAGScore:
```
Run ./000_Code_Directory/PREDICT_Code/FRAGScore/offtarget_fragscore.py, using bam files as input
```

3. IFScore:
```
Run ./000_Code_Directory/PREDICT_Code/IFScore/offtarget_ifs.py, using bam files as input
```

### The computed features for the SNVScore, FRAGScore, IFScore and PREDICT model construction in the retrospective cohort 
1. SNVScore:
```
./1_Model_Features/0_SNVScore_Input_Features
```

2. FRAGScore:
```
./1_Model_Features/1_FRAGScore_Input_Features
```

3. IFScore:
```
./1_Model_Features/2_IFScore_Input_Features
```

4. PREDICTScore: 
```
./1_Model_Features/3_PREDICTScore_Input_Features
```

### Code for computing the 12 machine learning performance metrics
```
Run ./2_ML_Performance_Metrics/0_Code_ML_metrics.r, using input "0_Input"
```
