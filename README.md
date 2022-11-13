# 문화체육관광부와 국립국어원이 개최한 "2022 국립국어원 인공지능 언어 능력 평가" 대회에 사용한 소스코드 및 데이터입니다.<br/>

## 1. 대회 설명
https://corpus.korean.go.kr/task/taskList.do?taskId=8&clCd=END_TASK&subMenuId=sub01
<br/>

## 2. Inference
https://drive.google.com/drive/folders/1cWGSYiGNeh0rL63ZdhQ0IpQkPvFnmPv3?usp=share_link <br/>
위 링크에서 Best_Models 압축파일 다운받은 후, Jupyter_version 폴더 아래에 Best_Models라는 폴더명으로 압축해제 후, Inference.ipynb 파일을 통해 결과 추출 가능합니다.<br/>
결과는 Result 폴더가 생성되면서 폴더 내에 pred.json으로 저장됩니다.

## 3. Train
Jupyter_version 폴더에 있는 aspect_category_classification.ipynb 파일 실행하여 Acc 모델 학습 -> Model/category_extraction 폴더 생성되면서 모델 추출<br/>
Jupyter_version 폴더에 있는 aspect_sentiment_classification.ipynb 파일 실행하여 Asc 모델 학습 -> Model/polarity_classification 폴더 생성되면서 모델 추출<br/>

## 4. Preprocess
Jupyter_version/Data preprocessing/data_preprocessing_acc.ipynb 파일 통해 ACC 모델에 쓰일 학습데이터 전처리 -> 전처리 결과 파일 Preprocessed_data/acc 폴더에 추출<br/>
Jupyter_version/Data preprocessing/data_preprocessing_asc.ipynb 파일 통해 ASC 모델에 쓰일 학습데이터 전처리 -> 전처리 결과 파일 Proerpocessed_data/asc 폴더에 추출<br/>
