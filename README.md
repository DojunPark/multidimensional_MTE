# Multi-Dimensional Machine Translation Evaluation: Model Evaluation and Resource for Korean

This repository contains resources developed for our research on Multidimensional Machine Translation Evaluation for the English-Korean language pair, as presented at [LREC-COLING 2024](https://arxiv.org/abs/2403.12666). It includes the `En_Ko_MQM_Quality_Scores.tsv` dataset and the `MTE_QE_model_training_code(RemBERT).ipynb` Jupyter notebook for model training.

## Dataset Description

### Overview

The `En_Ko_MQM_Quality_Scores.tsv` dataset comprises 1200 data points, leveraging the Multidimensional Quality Metrics (MQM) framework to evaluate translation quality across multiple dimensions.

### Data Structure

Each data point is formatted with the following columns:

- **type**: Data set categorization (training, validation, test).
- **corpus**: Origin corpus (Global Voices, TED Talks).
- **en_source**: English source sentence.
- **ko_reference**: Korean reference translation.
- **ko_target**: Korean translated sentence.
- **annotation**: MQM error annotations.
- **accuracy**: Translation accuracy score.
- **fluency**: Translation fluency score.
- **style**: Style consistency score between source and target.
- **total**: Aggregate MQM score.

### Splits

- **Training Set**: 0 to 1000
- **Validation Set**: 1001 to 1100
- **Test Set**: 1101 to 1200

This dataset is instrumental for research in machine translation quality estimation, especially for those looking into the nuanced evaluation of translations beyond single-score metrics.

## Model Training Code

The `MTE_QE_model_training_code(RemBERT).ipynb` Jupyter notebook contains Python code for training and evaluating models based on the RemBERT architecture for predicting MQM scores. The notebook illustrates:

- Data preprocessing steps for model input.
- Model training setup, including parameter configuration and training loop.
- Evaluation metrics and model performance assessment.

This code serves as a practical guide for researchers and practitioners aiming to replicate our study's findings or develop their models for multidimensional translation quality evaluation.

## Usage

### Dataset

Intended for academic and research purposes, this dataset allows for the development, testing, and comparison of models capable of multidimensional quality evaluation in machine translation, specifically for English to Korean translations.

### Model Training Code

Researchers can use the provided Jupyter notebook to understand the model training process, replicate our study's results, or adapt the code for their experiments on translation quality estimation.

## Citation

If you utilize the dataset or the model training code in your research, please cite our paper from LREC-COLING 2024:

```bibtex
@inproceedings{Park2024MultiDimensionalMT,
  title={Multi-Dimensional Machine Translation Evaluation: Model Evaluation and Resource for Korean},
  author={Dojun Park and Sebastian Pad'o},
  year={2024},
  booktitle={Proceedings of the LREC-COLING 2024},
  url={https://api.semanticscholar.org/CorpusID:268532121}
}
```
