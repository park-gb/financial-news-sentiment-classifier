# 한국어 경제 뉴스 기사 감정 분류
![Colab](https://user-images.githubusercontent.com/80144296/171107614-be32a03d-55a8-452e-9055-3d11452e40de.png)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
## 1. 개요
- 경제 뉴스 기사 문장의 감성(sentiment)이 긍정(positive), 중립(neutral), 부정인지 구분하는 텍스트 분류 프로젝트
- 사전 학습 언어모델인 KLUE BERT-base와 경제 뉴스 기사의 감정 데이터가 라벨링된 오픈소스 데이터셋인 [Finance Phrase Bank](Finance Phrase Bank) 활용

## 2. 사전 학습 언어모델(PLM)
- App 사용자 리뷰 데이터 수집
  - 리뷰 등록일
  - 작성자 닉네임
  - 리뷰 평점
  - 리뷰 내용
\

3# 4. 전체 파일구조
``` bash
├─financial-news-sentiment-classifier
│   Sentiment_Classifier_for_Kor_Financial_News
│   README.md
│   LICENSE
│   ├─data
│   │      dataset.csv
|   |      dataset_prep.csv
│   └─metric
│         cl_report.csv
│         metircs.csv
```

## 참고문헌
- 개인 블로그(Tistory): https://heytech.tistory.com
- Gitgub: https://github.com/park-gb/financial-news-sentiment-classifier

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
