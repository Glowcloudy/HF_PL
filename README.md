# HF_PL
# MTEB News Dataset

[Hugging Face: mteb/news](https://huggingface.co/datasets/mteb/news)

영문 뉴스 문장을 4개 토픽으로 분류한 데이터셋입니다. `datasets` 라이브러리로 바로 불러와 텍스트 분류(토픽 분류) 모델을 학습하거나 벤치마크에 사용할 수 있습니다.

## 빠른 정보 (Quick Facts)
- **언어(Language)**: English  
- **모달리티**: Text  
- **포맷**: Parquet  
- **샘플 수**: 약 **128k** rows  
- **스플릿**: `train` **119,958** / `test` **7,600**  
- **레이블(4 classes)**  
  - `0`: World  
  - `1`: Sports  
  - `2`: Business  
  - `3`: Sci/Tech  

## 스키마(Features)
| column | dtype  | 설명 |
|-------:|:------:|------|
| `text` | string | 뉴스 문장(헤드라인/요약 등) |
| `label`| int    | 클래스 라벨 ID (0~3), 아래 id→이름 매핑 참고 |

## 📊 Sentiment Analysis Summary (2025-08-28)

- **Source-wise average sentiment (−1 ~ +1)**: `-0.059126`
- **Date-wise average sentiment**: `2025-08-28 → -0.059126`

### 🏷️ Label distribution
| label    | count | share |
|:---------|------:|------:|
| neutral  | 2,598 | 51.96% |
| negative | 1,310 | 26.20% |
| positive | 1,092 | 21.84% |
| **total**| **5,000** | **100%** |

> Overall drift: slightly negative (`-0.059`).
