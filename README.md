# fastSNARE
## A sequence-based approach for identifying SNARE proteins by incorporating deep learning architecture and amino acid embedding representation

### Step 1
Install FastText package via the instructions here: https://github.com/facebookresearch/fastText

### Step 2
Use "fasttext_generated.py" file to transform FASTA sequence into FastText format
- *python fasttext_generated.py fasta_file fasttext_file*

### Step 3
Print vectors using FastText model:
- *fasttext print-sentence-vectors model.bin < fasttext_file > vector_file*

### Step 4
Use "fastsnare_train.py" to train and evaluate the generated file:
- *python fastsnare_train.py vector_file*

## Citation
Please cite our paper as follows:
>Le NQK and Huynh T-T (2019) Identifying SNAREs by Incorporating Deep Learning Architecture and Amino Acid Embedding Representation. *Front. Physiol.* 10:1501. doi: 10.3389/fphys.2019.01501
