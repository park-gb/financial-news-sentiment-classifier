# 한국어 경제 뉴스 기사 감정 분류
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
## 1. 개요
- Pretrained 언어 모델인 [KLUE BERT-base](https://github.com/KLUE-benchmark/KLUE) 위에 경제 뉴스 기사의 감정이 라벨링된 데이터셋 [한국어 버전의 Finance Phrase Bank](https://github.com/ukairia777/finance_sentiment_corpus/blob/main/finance_data.csv)을 활용하여 파인튜닝한 감정 분류 프로젝트
- 개발 환경: [Google Colab Pro / GPU](https://colab.research.google.com/signup)

## 2. Pretrained 언어 모델
- KLUE BERT base([Github](https://github.com/KLUE-benchmark/KLUE)/[Hugging Face](https://huggingface.co/klue/bert-base)/[논문](https://arxiv.org/pdf/2105.09680.pdf))

## 3. 경제 뉴스기사 감정 데이터셋
- 영문 데이터셋인 [Finance Phrase Bank](https://huggingface.co/datasets/financial_phrasebank)를 한국어로 번역하고 육안 검수한 데이터셋(출처: Github [@ukaria777](https://github.com/ukairia777/finance_sentiment_corpus/blob/main/finance_data.csv))
- 데이터 개수: 경제 뉴스기사 내 4,846개 문장

<img width="604" alt="sample_data" src="https://user-images.githubusercontent.com/80144296/171138476-694017b2-e8eb-4a0a-a4cf-fe342ca3bebb.png">


- 감정 라벨: Neutral(59.27%), Positive(28.22%), Negative(12.51%) 

![label_ratio](https://user-images.githubusercontent.com/80144296/171126744-b4215a97-afa4-4569-b56b-ac534541d6cc.png)

(라벨 정보) 0: Neutral, 1: Positive, 2: Negative

## 4. 파인튜닝 모델 성능
### 1) Confusion Matrix

![cf_matrix](https://user-images.githubusercontent.com/80144296/171126977-5f535777-2c91-42b4-a3c5-71d3b6c6d498.png)

### 2) Metrics

|Metric|Score|
|--------|-----|
|Accuracy|0.852|
|Precision|0.851|
|Recall|0.852|
|F1 Score|0.851|
|ROC AUC Score|0.920|
|Cohen's Kappa Coefficient|0.728|
|Matthews Correlation Coefficient  |0.729|
|Log Loss|0.555|

## 5. 전체 파일구조
``` bash
├─financial-news-sentiment-classifier
│   sentiment_classifier.ipynb
│   README.md
│   LICENSE
│   ├─data
│   │      dataset.csv
│   │      dataset_prep.csv
│   ├─figure
│   │      cf_matrix.png
│   │      label_number.png
│   │      label_ratio.png
│   └─metric
│         cl_report.csv
│         metircs.csv
```

## 프로젝트 상세 설명
- 개인 블로그(Tistory): https://heytech.tistory.com/394

## 📝 License
```
MIT License

Copyright (c) 2022 Gyeongbin Park

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
