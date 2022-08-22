# 안산부곡초 학생현황 대시보드

## 개요
- 개인적으로 학생현황을 확인하는데, 엑셀파일을 열어서 확인하는 것이 번거로움.
- 요약된 데이터 및 그래프를 웹에서 확인했으면 하는 바램에서 streamlit을 이용하여 대시보드 구현

## 주요기능
- 기간을 선택하여 인원 확인
- 학년, 반 선택하여 데이터 시각화
- 시각화 
  - 학년별 전체인원 시각화
  - 남녀 비율 원그래프 시각화

## 개발환경
- python 3.8.7
- 주요 라이브러리
  - pandas, streamlit

## 프로세서
1. 데이터 파일 읽어오기
2. 데이터 전처리
   1. 학년별 소계 삭제 및 인덱스 리셋
   2. 학년 칼럼에 학년 입력
   3. 남녀 합계 칼럼 생성
3. streamlit 환경 구성
   1. 사이드바 생성 : 학년, 반 선택 
   2. 메인페이지 생성
      1. 화면 4분할 : 데이터 요약
         1. 전체학급수
         2. 남학생 인원
         3. 여학생 인원
         4. 전체 인원
      2. 데이터 그래프 생성