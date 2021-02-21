# RNA-seq-ATAC-seq-analysis-pipeline

## 1. download pipeline.zip 
git clone https://github.com/Ting-PKU/RNA-seq-ATAC-seq-analysis-pipeline.git  

## 2. unzip downloaded files
cd RNA-seq-ATAC-seq-analysis-pipeline/  
tar -zvxf pipeline.tar.gz  
cd pipeline/  

## 3. Prepare ATAC-seq, RNA-seq count matrix and metadata as files in example/
ATAC_count.txt - count matrix of ATAC-seq  
RNA_count.txt - count matrix of RNA-seq  
ATAC_meta - metadata of ATAC-seq  
RNA_meta - metadata of RNA-seq  

## 4. run Deseq2_analysis.R
Rscript Deseq2_analysis.R --data_dir=/dir/of/your/count/matrix  

## 5. run network.R
Rscript network.R --motif_data_dir=/dir/of/the/motif/dir/after/step4  --TF='Hub TF' (eg. --TF=GRE)


