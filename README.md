# Bengali Pharmaceutical Product Review Dataset (BPRD)

## 📋 Overview

The **Bengali Pharmaceutical Product Review Dataset (BPRD)** is the first benchmark dataset for pharmaceutical product reviews in the Bengali language, comprising **9,515 expert-verified reviews** with five-star ratings. This repository provides the complete dataset together with the data splits and resources used in our study.

## 📊 Dataset Description

- **Total Reviews:** 9,515
- **Rating Classes:** 5 (1-star to 5-star)
- **Language:** Bengali
- **Domain:** Pharmaceutical Products
- **Source:** Multiple e-commerce platforms
- **Annotation:** Expert-verified with rigorous quality control

### Dataset Statistics

| Rating Class | Number of Reviews | Percentage |
|--------------|------------------:|-----------:|
| Rating 1 | 2,199 | 23.1% |
| Rating 2 | 1,563 | 16.4% |
| Rating 3 | 1,526 | 16.0% |
| Rating 4 | 1,989 | 20.9% |
| Rating 5 | 2,238 | 23.5% |
| **Total** | **9,515** | **100%** |

### Dataset Split

- **Training Set:** 6,660 reviews (70%)
- **Validation Set:** 952 reviews (10%)
- **Test Set:** 1,903 reviews (20%)

Stratified sampling was used to preserve the class distribution across all dataset splits.

---

## 📑 Dataset Format

Each sample in the dataset contains the following fields.

| Column | Description |
|---------|-------------|
| `review_id` | Unique review identifier |
| `review_text` | Bengali pharmaceutical product review |
| `rating` | Expert-verified rating (1–5 stars) |
| `product_category` | Pharmaceutical product category |
| `verified` | Expert verification status (`True`/`False`) |
| `split` | Dataset split (`train`, `validation`, or `test`) |

### Example

```csv
review_id,review_text,rating,product_category,verified,split
1,"এই ওষুধটি খুবই কার্যকর। ব্যথা দ্রুত কমিয়ে দেয়।",5,pain_relief,True,train
2,"খাওয়ার পর পার্শ্ব প্রতিক্রিয়া অনুভব করেছি।",2,antibiotic,True,train
3,"দাম অনুযায়ী ভালো পণ্য।",4,vitamins,True,validation
4,"কোনো উন্নতি লক্ষ্য করিনি।",1,pain_relief,True,test
```

---

## 🔬 Key Features

1. **Expert-Verified Dataset:** All ratings verified against review content.
2. **Rating Inflation Analysis:** Identified **16.20%** rating discrepancies.
3. **Multi-Stream Attention:** Novel architecture for pharmaceutical review classification.
4. **Comprehensive Baselines:** Comparison with traditional machine learning, deep learning, and transformer-based models.
5. **Explainability:** LIME and LIG analysis for model interpretability.
6. **Low-Resource Language:** Addresses challenges in Bengali NLP.

## 📧 Contact

For questions or issues, please contact:

- **Corresponding Author:** Aminur Rahman
- **Email:** aminurrahmanashik@gmail.com

## 📜 License

This dataset and code are released under the **MIT License**.

### Usage Terms

- ✅ Academic and research use
- ✅ Commercial use with attribution
- ✅ Modification and distribution
- ❌ Use for harmful purposes
- ❌ Redistribution without attribution

## 🙏 Acknowledgments

We thank the annotators and domain experts who contributed to the development and verification of this dataset.

## 🔄 Updates

- **v1.0** (January 2025): Initial release with 9,515 reviews.
- Future updates will be listed here.

---

> **Note:** This dataset is intended for research and educational purposes only. It should not be used as a substitute for professional medical advice.
