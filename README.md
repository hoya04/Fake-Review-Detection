# 트랜스포머 기반 가짜 리뷰 탐지기

## 프로젝트 개요
본 프로젝트는 Transformer 기반 임베딩(BERT 및 RoBERTa)을 활용한 가짜 리뷰 탐지 모델을 구현하고, 기존 전통적 방식(TF-IDF, Word2Vec)과의 성능을 비교합니다.

## 주요 기술
	- 임베딩: BERT, RoBERTa ([CLS] 토큰 벡터 사용)
	- 분류기: Dual-branch MLP → Dense + Dropout 구조
	- 성능 비교: Concatenate vs Multiply 조합, 전통 임베딩 기법과의 성능 비교

 
##  저장소 구성
- BERT,RoBERTa,Word2Vec
  - 0_data_preprocessint.ipynb : 전처리 코드
  - BERT_model.ipynb : BERT
  - RoBERTa.ipynb : RoBERTa
  - hybrid_model.ipynb : concatenate, multiply
  - word2vec_RNN_model.ipynb : word2vec + RNN

- TF-IDF
  - tf_idf_modeling.ipynb : tf-idf
  - Data_Preprocessing.ipynb 전처리 코드   
 ## 실행환경
- Python 버전: 3.9.21

## 주요 라이브러리 및 환경 정보
- transformers==4.41.2
- torch==2.3.0
- scikit-learn==1.3.2
- pandas==2.0.3
- numpy==1.24.3
- matplotlib==3.7.5
- seaborn==0.12.2
- tqdm==4.67.1
- nltk==3.9.1
- regex==2024.11.6
- jupyterlab==4.1.5
- ipykernel==6.29.4
