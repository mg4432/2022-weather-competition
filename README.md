# 2022 날씨 빅데이터 콘테스트 

<div align = center>

[<img src="https://user-images.githubusercontent.com/73567364/183577166-eedef0dc-822e-4ed1-94be-5c240c958cc9.png" width="700">](https://bd.kma.go.kr/contest/main.do)

</div>
  
## 1. 대회 설명
**2차 대회 2과제 : 기상에 따른 혈관질환 발생 예측 모델 개발**
- 기상청에서 제공하는 기상 데이터와 예보 데이터를 바탕으로 **일별, 지역별 혈관 질환으로 인한 입원 빈도**를 예측하는 과제입니다. 
- 최종공모안 파일에 EDA, 모델링, 활용 방안에 대한 설명이 있습니다. 

## 2. 순위
최종 순위 : 입선 (4위)
- RMSE (Validation set) : 1.2085

![image](https://user-images.githubusercontent.com/73567364/216526818-1f1bddc0-eeb8-4e81-9689-167f2e3647d9.png)

## 3. 사용 모델 : NgBoost

<div align = center>
  
[<img src="https://stanfordmlgroup.github.io/projects/ngboost/img/toy_single.png" width="500">](https://stanfordmlgroup.github.io/projects/ngboost/)
[<img src="https://stanfordmlgroup.github.io/projects/ngboost/img/toy_natural.gif" width="500">](https://stanfordmlgroup.github.io/projects/ngboost/)
  
</div>

### model description
**Base Learner**

The most common choice is Decision Trees, which tend to work well on structured inputs.

**Probability Distribution**

The distribution needs to be compatible with the output type. For e.g. Normal distribution for real valued outputs, Bernoulli for binary outputs.

**Scoring rule**

Maximum Likelihood Estimation is an obvious choice. More robust rules such as Continuous Ranked Probability Score are also suitable.

The above choices can be mixed and matched to be customized for the specific prediction problem at hand.


<div align = center>

[<img src="https://stanfordmlgroup.github.io/projects/ngboost/img/blocks.png" width="1000">](https://stanfordmlgroup.github.io/projects/ngboost/)

</div>
