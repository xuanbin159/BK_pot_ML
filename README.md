# BK_pot_ML
# Embedding & Autoencoder

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/xuanbin159/BK_pot_CL/blob/main/2_embedding_autoencoder.ipynb)

## 개요

본 저장소는 논문 *"Transforming Market Whitespaces into New Product Concepts: A Text Embedding and Inversion Approach"* (Journal of Engineering Design, https://doi.org/10.1080/09544828.2025.2568820) 에서 사용된 텍스트 임베딩 생성 및 Autoencoder 차원 축소 코드를 포함하고 있습니다. 전처리된 제품 설명 텍스트를 OpenAI API로 임베딩한 뒤, PyTorch 기반 Autoencoder를 통해 1536차원에서 2차원으로 축소하고 그 결과를 시각화합니다.

## 주요 구성

| 단계 | 내용 |
|---|---|
| 임베딩 생성 | OpenAI text-embedding-ada-002 모델을 활용한 텍스트 벡터화 |
| Autoencoder 학습 | 10층 인코더/디코더 구조, AdamW 옵티마이저, MSE 손실 함수 기반 학습 |
| 시각화 | 2차원 축소 결과 산점도 |

## 실행 환경

Google Colab 환경에서 실행되며, Google Drive 마운트와 OpenAI API 키가 필요합니다.

## 의존성

```
openai, torch, pandas, numpy, matplotlib
```
