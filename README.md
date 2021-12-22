# CyBERT: Contextualized Embeddings for the Cybersecurity Domain

This repository provides pre-trained weights of CyBERT, a language representation model for the cybersecurity domain. This model can be used for a variety of cybersecurity-based downstream tasks such as named entity recognition, and multi-class classification. 

Refer to the [published paper](https://ebiquity.umbc.edu/_file_directory_/papers/1117.pdf)  for more information, and please use the following citation below when testing and/or re-purposing provided materials:

## Citation
```
@inproceedings{ranade2021cybert,
  title={CyBERT: Contextualized Embeddings for the Cybersecurity Domain},
  author={Ranade, Priyanka and Piplai, Aritran and Joshi, Anupam and Finin, Tim and others},
  booktitle={IEEE International Conference on Big Data},
  year={2021}
}
```
## Downloading Models

Available model releases will be available here in the [Releases](https://drive.google.com/drive/folders/17B0DjdI3WRn0eAYe7ecF91gmN2Uj5FiB?usp=sharing) directory. Current model links are also available below:

* **[CyBERT-Base-MLM v1.1](https://drive.google.com/drive/folders/1MUpyXXjZTgvowjPt-FoD5hp2cwO95Oii?usp=sharing)** - fine-tuned on BERT-Base-Cased, with extended cybersecurity vocabulary.

## Fine-tuning CyBERT

To use CyBERT for fine-tuning cybersecurity tasks using the provided models, load the model and extended tokenizer using `Hugging Face` **from_pretrained module:

```
from transformers import BertTokenizer, BertForMaskedLM

tokenizer = BertTokenizer.from_pretrained("path to CyBERT directory")
model = BertForMaskedLM.from_pretrained("path to CyBERT directory")
```

# Contact information
For help or issues, please contact [Priyanka Ranade](priyankaranade@umbc.edu)
