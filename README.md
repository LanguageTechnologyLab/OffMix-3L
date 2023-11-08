# OffMix-3L: A Novel Code-Mixed Dataset in Bangla-English-Hindi for Offensive Language Identification

**Publication**: *The 11th International Workshop on Natural Language Processing for Social Media (SocialNLP) under AACL-2023.*

**Read in [arXiv](https://arxiv.org/pdf/2310.18387.pdf)** 

---

## 📝 Citation

When using the OffMix-3L dataset, please cite the following:

```bibtex
@article{goswami2023offmix,
  title={OffMix-3L: A Novel Code-Mixed Dataset in Bangla-English-Hindi for Offensive Language Identification},
  author={Goswami, Dhiman and Raihan, Md Nishat and Mahmud, Antara and Anstasopoulos, Antonios and Zampieri, Marcos},
  journal={arXiv preprint arXiv:2310.18387},
  year={2023}
}
```

---

## 📖 Introduction

Code-mixing is a well-studied linguistic phenomenon when two or more languages are mixed in text or speech. Several datasets have been built with the goal of training computational models for code-mixing. Although it is very common to observe code-mixing with multiple languages, most datasets available contain code-mixed between only two languages. In this paper, we introduce OffMix-3L, a novel dataset for sentiment analysis containing code-mixed data between three languages: Bangla, English, and Hindi.

---

## 📊 Dataset Details

We introduce **OffMix-3L**, a novel three-language code-mixed test dataset with gold standard labels in Bangla-Hindi-English for the task of Sentiment Analysis, containing 1,001 instances.

> We are presenting this dataset exclusively as a test set due to the unique and specialized nature of the task. Such data is very difficult to gather and requires significant expertise to access. The size of the dataset, while limiting for training purposes, offers a high-quality testing environment with gold-standard labels that can serve as a benchmark in this domain.

---

## 📈 Dataset Statistics

|                   | **All** | **Bangla** | **English** | **Hindi** | **Other** |
|-------------------|---------|------------|-------------|-----------|-----------|
| Tokens            | 87,190  | 31,228     | 6,690       | 14,694    | 34,578    |
| Types             | 18,787  | 7,714      | 1,135       | 1,413     | 8,645     |
| Max. in instance  | 173     | 62         | 20          | 47        | 93        |
| Min. in instance  | 41      | 4          | 3           | 2         | 8         |
| Avg               | 87.10   | 31.20      | 6.68        | 14.68     | 34.54     |
| Std Dev           | 20.58   | 8.60       | 3.05        | 5.74      | 10.98     |

*OffMix-3L Data Card. The row "Avg" represents the average number of tokens with its standard deviation in row "Std Dev".*


---

## 📉 Results

| Models         | F1 Score |
|----------------|----------|
| BanglishBERT   | **0.68** |
| BERT           | 0.66     |
| mBERT          | 0.63     |
| HingBERT       | 0.60     |
| MuRIL          | 0.60     |
| HateBERT       | 0.60     |
| fBERT          | 0.58     |
| roBERTa        | 0.58     |
| XLM-R          | 0.57     |
| DistilBERT     | 0.57     |
| GPT 3.5 Turbo  | 0.57     |
| BanglaBERT     | 0.54     |
| IndicBERT      | 0.55     |
| HindiBERT      | 0.43     |

*Weighted F-1 score for different models: training on synthetic and tested on natural data (OffMix-3L).*
