### [TOKEN is a MASK: Few-shot Named Entity Recognition with Pre-trained Language Models](https://arxiv.org/abs/2206.07841) 

This repository contains sample notebooks for both [zero-shot](https://github.com/uds-lsv/TOKEN-is-a-MASK/blob/main/example_zero-shot.ipynb) and [few-shot](https://github.com/uds-lsv/TOKEN-is-a-MASK/blob/main/example_few-shot.ipynb) scenarios based on [CoNLL-03](https://github.com/uds-lsv/TOKEN-is-a-MASK/tree/main/data/conll03NER), we did not use OntoNotes and i2b2 dataset because they are not publicly available. 

### Steps for Few-shot learning with "TOKEN is a MASK"
- Step 1: Train an NER model based on some small available labelled data e.g number of sentences, K=50 or 100. You can use the official [HuggingFace code](https://github.com/huggingface/transformers/tree/main/examples/pytorch/token-classification) for this. 
- Step 2: Combine it with the "TOKEN is a MASK" using the prediction file from Step 1. In the [example_few-shot.ipynb](https://github.com/uds-lsv/TOKEN-is-a-MASK/blob/main/example_few-shot.ipynb). We first trained for K = 100 sentences based on [conll2003_100](https://github.com/uds-lsv/TOKEN-is-a-MASK/tree/main/data/conll03_100), and save the prediction file in [output directory](https://github.com/uds-lsv/TOKEN-is-a-MASK/blob/main/output/test_predictions.txt). 


### BibTeX entry and citation info
```
@article{Davody2022TOKENIA,
  title={TOKEN is a MASK: Few-shot Named Entity Recognition with Pre-trained Language Models},
  author={Ali Davody and David Ifeoluwa Adelani and Thomas Kleinbauer and Dietrich Klakow},
  journal={ArXiv},
  year={2022},
  volume={abs/2206.07841}
}
```
