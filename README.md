# MeMI_ALFFEL_DATATHON
아이펠 데이터톤: 팀 MeMI_ICU 내 항생제 치료 전략 및 다제내성균(MDR) 감염의 치료 성공률 분석

<br>

## 팀원
<table>
  <tr>
    <td>
        <a href="https://github.com/KIID4">
         <img src = "https://avatars.githubusercontent.com/u/23628584?v=4" width="100px" />  
        </a>
    </td>
   <td>
        <a href="https://github.com/kakyungkim">
         <img src = "https://avatars.githubusercontent.com/u/84395053?v=4" width="100px" />  
        </a>
    </td>
    <td>
        <a href="https://github.com/hayannn">
         <img src = "https://avatars.githubusercontent.com/u/102213509?v=4" width="100px" />  
        </a>
    </td>
   <td>
        <a href="https://github.com/Jihyeon3717">
         <img src = "https://avatars.githubusercontent.com/u/184886431?v=4" width="100px" />  
        </a>
    </td>
  </tr>
  <tr>
    <td><b>👑안동균</b></td>
    <td><b>김가경</b></td>
    <td><b>이하얀</b></td>
    <td><b>손지현</b></td>
  </tr>
   <td><a href="https://github.com/KIID4">KIID4</a></td>
    <td><a href="https://github.com/kakyungkim">kakyungkim</td>
    <td><a href="https://github.com/hayannn">hayannn</td>
    <td><a href="https://github.com/Jihyeon3717">Jihyeon3717</td>
  </tr>
   <tr>
   <td><a href="https://velog.io/@kiid4/posts"/>velog</td>
    <td> - </td>
    <td><a href="https://velog.io/@dlgkdis801"/>velog</td>
    <td> - </td>
    
  </tr>
</table>





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

<br>

## 저장소 구조
```
├── 📑 README.md
|
├── 🗂 Info_MIMIC
|    └── 📑 MeMI_EDA.ipynb
|
├── 🗂 Subject01
|    ├── 📑 [keyword1차필터링]_MeMI_ICU_Analysis.ipynb
|    └── 📑 [keyword2차필터링+Optuna튜닝]_MeMI_ICU_Analysis.ipynb
|
├── 🗂 Subject02
|    └── 📑 [v3]project_2_temp.ipynb
|
└── 🗂 docs
     └── 🗂 TIL
     |    ├── 📑 TIL_241203_MIMIC_III_주제_관련_지표_분석.pdf
     |    ├── 📑 TIL_241204_ICU_환자의_항생제_사용과_치료_성공률_분석__다제내성균(MDR)_감염_치료_효과_분석.pdf
     |    ├── 📑 TIL_241204_SOFA.pdf
     |    ├── 📑 TIL_241204_중환자실에서의_다제내성균(MDR)_감염_치료_효과_분석.pdf
     |    ├── 📑 TIL_241205_Optuna_튜닝_적용(주제1).pdf
     |    └── 📑 TIL_241205_PPT_내용.pdf
     |
     ├── 📑 [Intro]MIMIC-III_Information_upload.pdf
     └── 📑 [MeMI]ICU_항생제치료전략_MDR_치료성공률.pdf


```

<br>

## 노트북 정보
- Subject 01.
  - `[keyword1차필터링]_MeMI_ICU_Analysis.ipynb` : 항생제 리스트업 1차 필터링 진행 노트북
  - `[keyword2차필터링+Optuna튜닝]_MeMI_ICU_Analysis.ipynb` : 항생제 리스트업 2차 필터링 진행 + Optuna 튜닝 진행 노트북

- Subject 02.
  - ♻️ `[v3]project_2_temp.ipynb` : 중환자실 내 다제내성균(MDR) 감염 치료 효과 분석 진행 노트북

- Info_MIMIC
  - `MeMI_EDA.ipynb` : EDA 관련 코드 및 시각화 진행 노트북

<br>

## 최종 발표 QnA 및 Feedback
### Subject 01 관련

#### 🙋 항생제를 사용하지 않은 경우의 수치는 고려하지 않은 것인지?
&nbsp;&nbsp;&nbsp;&nbsp; 🗣️ 우선, 고려하지 않음. 항생제의 사용 시 수치도 분류해서 같이 진행했다면 지표가 더 잘 나왔을 것 같아 아쉬운 부분. </tab>
> 피드백
> - 항생제 사용 시의 지표를 낸 만큼 **항생제 사용을 하지 않은 경우**도 컨트롤하는 지표도 함꼐 냈다면 더 유의미한 지표가 추출되었을 것.
> - 사용을 하지 않았지만 치료가 잘 된 케이스도 고려해야 함.

<br>

### Subject 02 관련
#### 🙋 치료가 되었다면 생존으로 지표가 추출되어야 하는 것이 아닌지?
&nbsp;&nbsp;&nbsp;&nbsp; 🗣️ "치료 효과"라는 정의 자체를 팀 내에서 정의한 정보이기 때문에, 나머지 지표에 따른 생존률의 차이가 있음.
<br>
&nbsp;&nbsp;&nbsp;&nbsp; 🗣️ 우선 사용한 MIMIC III 데이터에서 환자의 생체 정보와 관련된 중요 데이터를 구할 수가 없는 상황이었고 전체를 볼 수 있었던 약물 데이터에 조금 더 집중하여 주제를 선정하게 되었던 점이 더 다양한 전제를 고려하지 못한 부분으로 이어진 것 같아 아쉬움.

<br>

### 전체 Feedback
- 좋았던 점
  - 도메인 지식 및 데이터셋의 접근 권한 등의 문제가 있었음에도 가설과 전처리, 모델링의 처리 과정이 좋았고 고민을 많이 한 흔적이 느껴졌음.

- 아쉬운 점
  - 항생제 사용과 치료 성공 여부 : 항생제 종류에 따라서 효과가 다를 수 있는 부분이 있기 때문에 조금 더 분석해볼 수 있을 것.
  - MIMIC III 데이터셋에 대한 기본 정보에 대해서 조금 더 설명이 필요함.
    - `발표 시간 상의 문제와 더불어 데이터 설명에 대한 공식 자료가 많이 부족한 상태여서, 불필요한 내용을 제거하고 바로 데이터 처리에 대한 설명으로 들어갔던 점이 아쉽게 느껴지지 않았을까 하는 생각이 듦.`
