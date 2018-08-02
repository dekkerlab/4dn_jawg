# Dot calls

 - ESC dots called for biologicval replicates R1 and R2, and on a combined dataset R1+R2
 - HFFc6 dots called for biologicval replicates p17 and p22, and on a combined dataset p17+p22
 - GM12878 (Rao et al 2014) dots recalled using `cooltools` on a combined primary+replicate dataset
 - GM12878 dot calls by HiCCUPS (Rao et al 2014) can be found at https://www.ncbi.nlm.nih.gov/geo/download/?acc=GSE63525&format=file&file=GSE63525%5FGM12878%5Fprimary%2Breplicate%5FHiCCUPS%5Flooplist%2Etxt%2Egz
  
  
  
 https://github.com/dekkerlab/cooltools/commits/new-dotfinder

```
cooltools call_dots -n 12 \
    -o output.bedpe -v --fdr 0.1 \
    --max-nans-tolerated 7 \
    --max-loci-separation 10000000 \
    --dots-clustering-radius 21000 \
    --tile-size 2000000 \
    input.cool input-expected.csv
```
