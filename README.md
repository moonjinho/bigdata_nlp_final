# bigdata_nlp_final
빅데이터자연어처리기술 한글 감정분석 기말 과제

- 소스 실행 순서

1. git 소스에 있는 ratings_train.txt - 학습용 / ratings_test.txt - 테스트용 파일 준비
2. 필요한 라이브러리 import 및 데이터 가져오기
3. 훈련용 데이터 전처리
4. 테스트용 데이터 전처리
5. 정수 인코딩
6. 단어 분포 확인 후, 3회 미만으로 사용된 단어들은 제거
7. 토크나이징
8. label 값들 저장 후, 빈 샘플들 제거
9. 서로 다른 길이의 샘플들의 길이를 동일하게 작업 (패딩)
10. 단어 샘플들의 분포 비율 확인 후, max_len 30으로 설정
11. LSTM으로 리뷰 감성 분류 시작
12. 가장 좋은 모델을 기준으로 테스트 데이터 정확도 측정 (기준 val_acc)
13. Kaggle Sample 데이터를 통한 결과 분류 시작
14. sample.csv 파일로 export

- 참고한 오픈 소스

1. https://wikidocs.net/44249
2. https://wikidocs.net/31766
3. https://myjamong.tistory.com/77
4. https://wikidocs.net/92961
