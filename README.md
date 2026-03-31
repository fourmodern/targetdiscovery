# AI 기반 약물 표적 발굴

암 유전체 데이터, 그래프 신경망, 공개 데이터베이스, LLM을 활용하여 약물 표적을 발굴하는 실습 자료입니다. 비소세포폐암(NSCLC)을 주요 사례로 다룹니다.

---

## 노트북 목록

| 번호 | 주제 | 설명 | Colab |
|------|------|------|-------|
| 01 | TCGA 데이터 분석 | TCGA 데이터베이스에서 폐암 RNA-seq 데이터를 가져와 차등 발현 유전자 분석, PCA, 생존 분석, pathway 분석 수행 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fourmodern/targetdiscovery/blob/main/01_mod.ipynb) |
| 02 | GNN 기반 표적 발굴 | PyTorch Geometric의 그래프 신경망(GNN)으로 유전자 간 관계를 그래프로 모델링하고 약물 표적 후보 예측 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fourmodern/targetdiscovery/blob/main/02_deeplearning.ipynb) |
| 03 | OpenTargets 폐암 표적 | OpenTargets GraphQL API로 폐암 연관 표적, 약물, 유전자 발현 데이터를 조회하고 우선순위 스코어링 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fourmodern/targetdiscovery/blob/main/03.OpenTargets_LungCancer_Patched.ipynb) |
| 04 | LLM Co-Scientist | LangChain + LangGraph + Google Gemini로 NSCLC 표적 탐색 AI 에이전트를 구성하여 문헌 분석 자동화 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fourmodern/targetdiscovery/blob/main/04_nsclc_llm_coscientist.ipynb) |

강의 슬라이드 PDF 2종이 저장소에 포함되어 있습니다.

---

## 실행 환경

모든 노트북은 Google Colab에서 바로 실행할 수 있습니다.

| 항목 | 내용 |
|------|------|
| 런타임 | Python 3.10 이상 |
| GPU | 02번(GNN) 실행 시 권장 |
| API 키 | 04번 실행 시 Google Gemini API 키 필요 (`GOOGLE_API_KEY`) |

04번 노트북 실행 시 API 키를 `getpass`로 입력하게 되어 있습니다. Colab 사이드바의 "보안 비밀(Secrets)"에 등록하거나 실행 중 직접 입력하세요.
