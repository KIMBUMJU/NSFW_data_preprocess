# NSFW_data_preprocess
## NSFW 텍스트 판별을 위한 모델용 데이터 전처리

### 🗂️ data
- **🗄️ unsmile_train_v1.0**: 모델에 직접 들어갈 데이터 형식의 데이터
  - **columns**
      1. **문장**: 판별 될 문장
      2. **기타 columns**: 
         - `['문장', '여성/가족', '남성', '성소수자', '인종/국적', '연령', '지역', '종교', '기타 혐오', '악플/욕설', 'clean']`

- **🗄️ HateScore**: unsmile 데이터셋과 결합 예정인 추가 데이터
  - **columns**
      1. **comment**: 판별 될 문장
      2. **macrolabel**: 대분류, `['혐오발언', '단순 악플', 'Clean']`
      3. **microlabel**: 소분류, unsmile 데이터셋과 직접적인 연관
      4. **source**: 데이터 출처

