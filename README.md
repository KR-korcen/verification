모든 비속어/욕설 판별기의 대한 성능을 비교합니다.
# 데이터
- [korean-malicious-comments-dataset](https://github.com/ZIZUN/korean-malicious-comments-dataset): 한국어 악성댓글 데이터셋 (10,000문장)
- [Curse-detection-data](https://github.com/2runo/Curse-detection-data): 각종 커뮤니티 사이트의 댓글의 욕설 여부를 분류한 한글 데이터셋 (5,825문장)
- [kmhas_korean_hate_speech](https://huggingface.co/datasets/jeanlee/kmhas_korean_hate_speech): 온라인 뉴스의 댓글를 8가지로 세분화하여 분류한 데이터셋 (78,978문장)
- [Korean Extremist Website Womad Hate Speech Data](https://www.kaggle.com/datasets/captainnemo9292/korean-extremist-website-womad-hate-speech-data/data): 한국 극단주의 웹사이트의 데이터를 분류한 데이터셋 (2,081문장)
- [LGBT-targeted HateSpeech Comments Dataset (Korean)](https://www.kaggle.com/datasets/junbumlee/lgbt-hatespeech-comments-at-naver-news-korean): 네이버 뉴스 성소수자 관련 댓글을 분류한 데이터셋 (8,837문장)

# 모델
> PYHTON
- [korcen](https://github.com/KR-korcen/korcen): 키워드 기반 비속어 판단 모듈
- [korcen-ml](https://github.com/KR-korcen/korcen-ml/blob/main/README.md): korcen으로 분류한 데이터를 학습한 딥러닝 기반 비속어 판별 모델
- [badword_check](https://github.com/Nam-SW/badword_check): 입력한 글(한글)이 욕설인지 아닌지를 딥러닝을 통해 판별하는 모델
- [CurseDetector](https://github.com/mangto/CurseDetector): 한글 유사도와 한글 발음 유사도를 이용한 욕설/비속어/금지어 필터링
> C

> JAVA

> JAVASCRIPT

> etc....


# 성능 검증
> 데이터와 결과가 일치한 개수 / 전체 데이터 개수

|  | [korean-malicious-comments-dataset](https://github.com/ZIZUN/korean-malicious-comments-dataset) | [Curse-detection-data](https://github.com/2runo/Curse-detection-data) | [kmhas_korean_hate_speech](https://huggingface.co/datasets/jeanlee/kmhas_korean_hate_speech) | [Korean Extremist Website Womad Hate Speech Data](https://www.kaggle.com/datasets/captainnemo9292/korean-extremist-website-womad-hate-speech-data/data) | [LGBT-targeted HateSpeech Comments Dataset (Korean)](https://www.kaggle.com/datasets/junbumlee/lgbt-hatespeech-comments-at-naver-news-korean) | 문장당 평균 처리 속도 |
|------|------|------|------|------|------|------|
| [korcen](https://github.com/KR-korcen/korcen) | 0.7121 | **0.8415** | 0.6800 | 0.6305 | 0.4479 | **11ms** |
| [korcen-ml](https://github.com/KR-korcen/korcen-ml/blob/main/README.md)(free)(23.5.28) | 0.7545 | 0.7824 |  | 0.7055 | 0.6875 | 45ms |
| [korcen-ml](https://github.com/KR-korcen/korcen-ml/blob/main/README.md)(paid)(24.1.29) | **0.8322** | 0.8410 | **0.7837** | **0.7120** | **0.7477** | 38ms |
| [badword_check](https://github.com/Nam-SW/badword_check)(23.10.1) | 0.5829 | 0.6761 |  | 0.6410 | 0.4738 | 43ms |
| [CurseDetector](https://github.com/mangto/CurseDetector)(24.1.10) | 0.5679 |  |  | 0.5785 |  | 267ms |

# 테스트 환경
> i7-11800H @ 2.30GHz
> 32GB 3200MHZ
> RTX 3060 Laptop
