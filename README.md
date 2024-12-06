# MeMI_ALFFEL_DATATHON
아이펠 데이터톤: 팀 MeMI_ICU 내 항생제 치료 전략 및 다제내성균(MDR) 감염의 치료 성공률 분석

<br>

## 팀원 소개
| [👑안동균]() | [김가경]() | [이하얀](https://github.com/hayannn) | [손지현]() |
|:-----------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------:|
|  ![안동균](https://github.com/user-attachments/assets/9b93a4cb-722d-4196-b537-5488c663c1e5)  |  ![image](https://github.com/user-attachments/assets/525cd00d-a760-46bb-9b3f-637b1e1cd196) | ![image](https://github.com/user-attachments/assets/fb2de7ba-8053-48b0-8529-0778a1b8cac7)  | ![image](https://github.com/user-attachments/assets/56537ffe-17e9-45ed-81ab-6e88da523c27) |


<br>

## 주제
ICU 내 항생제 치료 전략 및 다제내성균(MDR) 감염의 치료 성공률 분석

<br>

## 사용 데이터셋
- MIMIC III
  - MIMIC-III 데이터셋은 ICU에 입원한 5만 명 이상 환자들의 임상 기록, 생리학적 측정, 처방 정보, 검사 결과, 약물 처방 기록 등 다양한 의료 정보를 포함함
  - 데이터 수집 기간 : 2001년 ~ 2012년
  - 25개의 CSV 파일 존재  <br>
![image](https://github.com/user-attachments/assets/6f2fed3c-5562-4986-ae26-aa3239e409df)

<br>

## 노트북 정보
- Subject 01.
  - `[keyword1차필터링]_MeMI_ICU_Analysis.ipynb` : 항생제 리스트업 1차 필터링 진행 노트북
  - `[keyword2차필터링+Optuna튜닝]_MeMI_ICU_Analysis.ipynb` : 항생제 리스트업 2차 필터링 진행 + Optuna 튜닝 진행 노트북

- Subject 02.
  - 노트북 정보 기입
