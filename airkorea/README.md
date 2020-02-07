# 미세먼지 데이터

- ### station_list 폴더 : 각 측정소의 시각 별 미세먼지 데이터 (.csv)

  - ##### 2016년 ~ 2019년 / 1월 ~ 12월 / 1시 ~ 24시

- ### 05번 .ipynb : 측정소 이름은 사이트에서 직접 넣고, 데이터 다운로드와 csv 파일 변환은 자동

- ### 07(2)번 .ipynb : 아래와 같은 코드를 통해 hangangdaero라는 2차원 리스트 생성.

  ```python
  hangangdaero = make_si_list(df1, 10) # DataFrame, pm
  ```

- #### 측정소명[시각] 리스트에 그 측정소에서 한 달동안 특정 시각마다 측정한 미세먼지 데이터가 입력되어있음.

  ```python
  df1 = read_csv_ym('Yongsan_Hannamdaero','2019','1') # station,year,month
  hannamdaero= make_si_list(df1, 10) # DataFrame, pm
  hannamdaero[13] # time
  ```

  ##### '한남대로 측정소'에서 '2019'년 '1'월 매일 '13'시에 측정한 'pm10' 데이터.

- #### plot
  <img src="ex1.png" width="350" height="250"></img>
