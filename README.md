# 서울시 공공데이터를 대상으로 한 도메인 특화 Text2SQL 모델 개발
- 2024-1 졸업 프로젝트(정보통신 종합설계)
<img width="1702" alt="웹_Demo" src="https://github.com/user-attachments/assets/d8ac6a96-10e5-4cd9-95d0-6c62bbbb4e59" />

## 프로젝트 소개
- (주)카카오의 Text2SQL 오픈소스 모델인 RYANSQL의 성능 지표를 개선하고,
자연어를 입력받아 SQL 쿼리를 출력하는 웹사이트를 구현

## 프로젝트 기간
- 24.02 - 24.06

## 학습 환경
1. OS
  - Linux : Ubuntu 20.04.5 LTS
2. HW
  - GPU : NVIDIA RTX A6000
  - RAM : 128GB
3. SW
  - Python 3.8.10
  - PyTorch 2.2.2
  - CUDA Toolkit 12.1
  - Django 5.0.6

## 데이터셋
- AIHUB 자연어 기반 질의(NL2SQL) 검색 생성 데이터

## 데이터 파이프라인
<img width="1072" alt="image" src="https://github.com/user-attachments/assets/6262b18d-91c5-408e-bbdd-9d75df414f19" />

## 최종 결과
- sql query 난이도 별 성능 

| Hardness   | Easy | Medium | Hard | Extra Hard | All  |
|------------|------|--------|------|------------|------|
| 개선 전       | 90.5 | 84.8   | 81.3 | 17.5       | 80.8 |
| 개선 후       | 91.8 | 86.1   | 84.2 | 18.6       | 82.5 |

