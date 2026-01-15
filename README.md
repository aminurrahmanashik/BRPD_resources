# Bengali Pharmaceutical Product Review Dataset (BPRD)


## 📋 Overview

The Bengali Pharmaceutical Product Review Dataset (BPRD) is the first benchmark dataset for pharmaceutical product reviews in Bengali language, comprising 9,515 expert-verified reviews with five-star ratings. This repository provides the complete dataset along with code for all experiments reported in our paper.

## 📊 Dataset Description

- **Total Reviews:** 9,515
- **Rating Classes:** 5 (1-star to 5-star)
- **Language:** Bengali
- **Domain:** Pharmaceutical products
- **Source:** Multiple e-commerce platforms
- **Annotation:** Expert-verified with rigorous quality control

### Dataset Statistics

| Rating Class | Number of Reviews | Percentage |
|--------------|------------------|------------|
| Rating 1     | 2,199            | 23.1%      |
| Rating 2     | 1,563            | 16.4%      |
| Rating 3     | 1,526            | 16.0%      |
| Rating 4     | 1,989            | 20.9%      |
| Rating 5     | 2,238            | 23.5%      |
| **Total**    | **9,515**        | **100%**   |

### Dataset Split

- **Training Set:** 6,660 reviews (70%)
- **Validation Set:** 952 reviews (10%)
- **Test Set:** 1,903 reviews (20%)

Stratified sampling was used to maintain class distribution across all splits.

```

Expected results:
- **Machine Learning (Best):** Logistic Regression - 87.23% F1-score
- **Deep Learning (Best):** CNN+BiLSTM - 89.45% F1-score
- **Transformers (Best):** XLM-RoBERTa - 92.30% F1-score
- **Proposed Model:** Multi-Stream Attention - **93.10% F1-score**


Example:
```csv
review_id,review_text,rating,product_category,verified,split
1,"এই ওষুধটি খুবই কার্যকর...",5,pain_relief,True,train
2,"পার্শ্ব প্রতিক্রিয়া অনেক...",2,antibiotic,True,train
```

## 🔬 Key Features

1. **Expert-Verified Dataset:** All ratings verified against review content
2. **Rating Inflation Analysis:** Identified 16.20% rating discrepancies
3. **Multi-Stream Attention:** Novel architecture for pharmaceutical review classification
4. **Comprehensive Baselines:** Comparison with 15+ baseline models
5. **Explainability:** LIME and LIG analysis for model interpretability
6. **Low-Resource Language:** Addresses challenges in Bengali NLP


## 📧 Contact

For questions or issues, please contact:
- **Corresponding Author:** Aminur Rahman - aminurrahmanashik@gmail.com

## 📜 License

This dataset and code are released under the [MIT License](LICENSE). 

### Usage Terms

- ✅ Academic and research use
- ✅ Commercial use with attribution
- ✅ Modification and distribution
- ❌ Use for harmful purposes
- ❌ Redistribution without attribution

## 🙏 Acknowledgments

We thank the annotators and domain experts who contributed to dataset development. 


## 🔄 Updates

- **v1.0** (January 2025): Initial release with 9,515 reviews
- Future updates will be listed here

---

**Note:** This is a research dataset. For medical advice, please consult healthcare professionals.
