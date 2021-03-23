---
layout: default
---

This webpage provides all the useful information I wish to know when starting my journey in discovering scRNA-seq data.

# Distribution of UMI counts

For single cell RNA seq data, what are the distribution of the raw data? Does it depend on the patient, sample, tissue type, cell type, etc? The content below may answer this question.

# Does freezing affect the quality of the scRNA seq data?
A paper published in Genome Biology in 2020 by E. Madissoon et al studies the effect of cold storage on fresh healthy spleen, esophagus and lung from 5 donors over 72h. The authors observe a decrease in the proportions of lung T cells at 72h, higher percentage of  mitochondiral reads, and increased contamination by background ambient RNA reads in the 72-h samples in the spleen. The paper is available [here](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1906-x). 


The paper also indicate that tissue preservation for upto 24 hours prior to scRNA-seq is robust. 

# What is the efficiency of current scRNA-seq protocols?

The most used protocol in the market at the moment is 10X chromium. 
- The cell recovery rate is uncertain as indicated in the 10x protocol. And so the target cell number is only indicative.
- The rate of doublets increases with targeted number of recovered cells. For example, if the number of recovered cells is 500, the multiplet rate is around 0.4%, but it the recovered cell number is 10000, the rate is ~7.6%.
- 

# What are the techniques to preprocess scRNA-seq data, and why are they used?

# scRNA-seq integration using mutual nearest neighbors (MNN). What are the assumptions?
- The same population exists in both samples. 
- The batch effect variation is much smaller than the biological variation in the data set. This is reasonable. Consider the case where the batch effect is similar to the variation between cell types. Then, there is the possibility that the MNN algorithm will assign a cell to the wrong nearest neighbors. 
- The batch effect is orthogonal to the biological subspace. This roughly means that the biological effect and the batch effect should be some how independent. Examples: if one of the samples is affected by one gene that does not effect the cell-type identification. Then the integration can work for the cell-type identification analysis. 
 


[Tests for some markdown languages](./test.html)


[My lab book](./another-page.html).


[Machine Learning](./machinelearning.html).


[Digital Pathology](./newpage.html)


