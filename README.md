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
