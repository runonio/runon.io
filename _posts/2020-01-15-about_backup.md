---
layout: post
title: about 백업, 
date:   2020-01-01 06:32:00 +0000
author: macle
tags: trading
---

엔진 개발 과정에서 지식이 더 많아져서 초기사업 목표를 재 설정하였습니다. 사업화는 엔진의 완성도가 더 높아지고 다시 고민할 문제로 보여서 초기에 작성했던 내용 백업용 입니다.




## 개발의 필요성 인식

처음 투자를 해야 겠다고 생각이 들었던 건 급격하게 오르는 자산들의 가격을 보았을 때 입니다. 퀀트 시스템의 필요함을 느꼇을때는 당시에 매일 야근이 일상인 회사생활에서 직장생활과 투자는 병행할 수 없다고 느낀 시점 이었습니다.
회사에 다니면서는 제대로된 자산 시장의 공부를 할 여유가 없고 그때 그때 감정적인 대응으로 인해 손해를 볼 확율이 높다고 생각했습니다.

그래서 급여가 들어오면 생활비를 빼고 자산운용사에 자산을 매일 적립하는 방법이 좋을지 고민했지만 믿음이 가는 펀드매니저는 주변에 없었습니다.

정부부채, 기업부채, 가계부채, 통화량은 계속 늘어나고 인플레이션은 발생할 수 밖에 없고 유도 하기도 합니다. 예적금은 내 돈의 가치를 지켜주지 못합니다.

이 상황에 대해서 고민한 내용을 블로그에 작성한적이 있어서 아래에 링크합니다.

● [퀀트 추천언어와 직접개발 이유(링크)](https://runon.io/2024/03/19/language_reason/)

## 초기목표의 실수

런온 개발의 초기목표는 일반인이 경제적 지식을 알지 못해도 펀드매니저 이상의 자산관리를 할 수 있는 플랫폼 개발이었습니다. 직장인은 직장 생활에 집중할 수 있고, 직장업무보다 더 어려운 투자를 하기위한 노력을 여가 시간으로 만들어 주자는게 취지였고 저 또한 그런 환경을 원했습니다.

## 문제의 발견

플랫폼을 만들기 위해 자산시장 공부를 하다보니 트레이딩이란 시장이 아직 효율적이지 못한(비효율적) 부분에서 수익을 보는것이고, 시장이 효율적이라면 기대 수익은 시장 수익률이겠구나 라는 생각을 하게 되었는데 이부분에서 문제가 발생했습니다.

모두가 같은 방식의 로보어드바이저를 사용하면 비효율적인 시장은 빠르게 효율적으로 변하게 될거니 사업으로서의 성장성은 한계가 명확하겠구나 라는 생각이 들게 되었고 최근에 이러한 생각을 정리하는 글을 하나 작성한게 아래내용입니다.

● [로보어드바이저 및 퀀트 사업화에 대해서(링크)](https://runon.io/2024/04/14/roboadvisor_business/)

## 좋은 퀀트 로보어드바이저가 갖추어야 할 기능들

이부분은 제가 공부하면서 만든 경험으로 작업예정 항목에 있거나 구현하고 있는 필요하다가 생각되는 기능들입니다.
<br/>
변화하는 시장에서 시장의 비효율성을 빨리 찾아서, 잘 대응하고 리스크를 피하려면 아래의 기능들이 필요하다고 생각합니다.

#### 전략 생성의 편의성
인프라에서 다양한 데이터를 사용하고, 전략의 생성이 편리하게 자동화된 기능을 제공해야 합니다.

인프라에서는 분석에 필요한 데이터가 계속 추가 되는 환경이라고 생각해야하고, 다양한 데이터를 사용해서 전략을 자동설정 혹인 추천하는 기능 제공 (아직 추상적이라 개발 이 더 진행되면 명확해 질 것으로 예상)
#### 시장 변화를 잘 감지할 수 있는지
변화만 잘 감지해도 자동매매를 멈추고 그때그때 전략을 수정할 수 있을것 입니다.
<br>
추세 추종 전략은 박스권에서는 반대로 동작하기 떄문에 추세 추종 전략을 사용한다면 이를 피할 수 있는 성능이 좋아야 합니다.
#### 손실제한 분할매수 분할매도에 대한 알고리즘 성능이 좋은지 시장가로 비싸게 사지않는게 구현되어있는지
리스크 관리의 중요성은 아무리 강조해도 지나치지 않습니다. 시스템으로 매매할때의 가장좋은 장점중 하나가 리스크 관리라고 생각합니다. 이부분의 편의성과 성능이 좋아야 합니다.
#### 리벨런싱 기능이 있는지, 여러 자산관리가 편한지
S&P 500은 장기적으로 우상향을 하였고 여러 주식은 편입 편출, 리벨런싱 합니다. 이러한 기능을 개인도 쉽게 할 수 있게 제공되면 좋은시스템일거 같네요.
#### 분석 해볼 수 있는 다양한 데이터 군을 기간별로 제공하는지
로보어드바이저나 퀀트는 가격과 거래량 이외에도 커뮤니티, 암화화폐 지값이동내역, 자동차 판매실적, 게임인기 매출순위 등과 같은 다양한 대안 데이터를 활용할 수 있습니다.
<br>
기간별로 데이터가 제공되어야 생존편향과 같은 벡테스팅의 오류를 줄일 수 있습니다.

#### 여러계좌 관리를 할 수 있는지
전략별로 다른 계좌를 활용하는 경우가 있습니다.
#### 벡테스팅에 슬리피지나 레이턴시, 분할매수 매도를 테스트해볼 수 있는지, 백테스팅 오류를 해결할 데이터군이 있는지
벡테스팅은 전략만을 테스트해서 위 기능이 구현되어 있지 않은 경우가 많지만 이기능까지 구현되면 다양한 실험을 해볼 수 있습니다.
<br>
생존편항, 미래참조편향을 과최적합 등에 대한 고려가 있는지 체크해볼 수 있습니다.

[ 벡테스팅 오류 와 해결방안(링크)](https://runon.io/2024/04/24/bacltestomg_error/)
#### 리스크 관리기능의 대양한 제공
리스크 관리는 여러 전략이 있을 수 있습니다. 아래에서 설명하는 전략은 예시입니다.

##### 손실제한, 혹은 연속손실이 발생했을때 자동매매를 멈추는 기능
트레이더도 장이 맞지 않으면 시장에 덤비지 않고 매매를 멈춤니다

##### 자산을 나누어 여러 전략의 매매봇을 이용하는 기능
트레이더는 1년에 50%는 물갈이 된다고 합니다.
봇도 실적이 좋지 않은 봇은 멈추고 실적이 좋은 봇 위주로 물갈이 되면서 돌아갈 수 있습니다.

#### 적용할 수 있는 시장이 많은지
국내거래소, 해외거래소, 암호화폐거래소와 앞으로 생길 많은 시장에 적용할 수 있다면 전략을 만들면 바로 사용할 수 있습니다.
#### 머신러닝 활용
전진분석이 포함된 머신러닝 이부분은 아직까지는 명확하게 정의하지 못했지만 목표에는 있는 기능이라 적어놓았습니다.

## 퀀트투자의 허와실, 과대광고 조심하기

좋지 않은 사례가 많이 보도되면서 관련 시장에 대해서 부정적인 시각이 많아 정리하고자 한 내용입니다.

● [퀀트 투자의 허와 실(링크)](https://runon.io/2024/04/09/quant_good_bad/)
<br/>
● [투자대회 고수익, 프로그램 고수익을 조심해야 하는 이유(링크)](https://runon.io/2024/04/12/high_profit_advertising/)

<br/>
<br/>
<br/>

## 초기 about

아래는 런온 개발을 처음 기획했을때 작성한 자료입니다. 지금은 목표가 많이바뀌었지만 보존용으로 남깁니다.

### 가치 보존
예적금은 가치를 지켜주지 못합니다.

● 현금가치 하락(인플레이션) <br/>
● 노동가치(인금상승률 - 인플레이션) <br/>
● 실질금리(명목금리 - 인플레이션) <br/> <br/>

### 현실적인 문제
투자를 잘하기 위해서는 기본적 분석, 기술적 분석, 거시경제학(매크로)등 많은 공부가 필요합니다. 하지만 직장 생활, 사업과 같은 생산활동을 하면서 좋은 투자를 하기는 어렵습니다. 많은 사람들이 도박성 단기투자로 손실을 보고 있습니다.<br/>

### 신뢰도 문제
투자전문가, 자산운용가에 대한 신뢰도가 낮아서 직접투자를 선호하고 있습니다. <br/>

### 개인화
투자금액, 투자기간, 투자성향은 개인에 따라 다르기 때문에 개인화가 필요합니다. <br/>

 <br/>

## 사업모델
### 자산운용
회사 자본금, 사업이익, 고객위탁금 운용 <br/>

### 데이터 분석 플랫폼 납품 (B2B)
자산관련 데이터가 있는 자산운용사, 증권사, 개인에 제품제공 <br/>

### 데이터 분석
데이터 분석을 외로 받아서 분석보고서 생성  <br/>
### 투자전략 중개
플랫폼에서 생성한 전략중개, 전략등록 수수료 전략등록 유지비용 <br/>
전략제공자는 다른 사용자에게 사용료를 받는구조, 사용료의 일정비율 <br/>

### 투자정보 사이트 운영 (B2C)
investing, tradingview, tradingeconomics 과 같은 투자 정보 사이트 운영 <br/>

 <br/>

## 비전
### 시장규모
자산시장의 전체 규모는 인플레이션이 존재하므로 계속 커지는 구조 입니다. <br/>
자산시장의 종류는 암호화폐를 시작으로 점점 더 많아 질 것으로 예상합니다. 부동산, 음악 저작권, 웹사이트같은 자산도 지분화 혹은 토큰화 구조로 변할 수 있습니다. <br/>
준비중인 데이터 분석 플랫폼은 데이터를 표준을 정의하여 사용하기 때문에 새로운 시장이 생겨도 빠른 적용이 가능합니다. <br/>

### 데이터 및 기술 누적
시간이 지나고나면 경쟁 우위에 있는 회사들만 남게되고 많은 회사가 사라지게 되는데, 지금도 연관분야 회사가 많고 아직도 생기고 있는 것으로 보아서는 특별하게 앞서고 있는 사업체는 없다고 보입니다.<br/>
빅데이터 처리, AI 기술이 자리잡고 있는 지금이 새롭게 도전하기에 좋은 시기 입니다. <br/>
데이터와 기술이 누적될 수록 인건비 감소로 수익구조는 점점 계선됩니다. <br/>

### 편리한 분석 도구를 기반한 증권사 혹은 거래소 설립
편리한 분석 도구를 기반한 증권사 혹은 거래소를 설립하는 경우와 같은 연계사업들이 계속하여 생길 수 있습니다. <br/>
분석플랫폼의 지금의 HTS에서 자산관리와 자동매매, 벡테스팅, AI 기능들이 추가된 형태로 개발하고 있습니다. <br/>
주식,원자재,암호화폐,선물,부동산, 계속해서 생길 많은 자산시장까지 편하게 관리하는 형태가 될 것으로 예상합니다.

 <br/>

## 가치
### 기술 기반 자산운용 회사
암호화폐 시장의 자산운용 비상장 회사의 가치가 최대 8000억 까지 인정받은 사례가 있습니다. <br/>
운용하고 있는 자산이 클수록, 운용할 수 있는 자산규모가 클수록, 기술경쟁력이 높을 수록 가치는 점점 높아집니다. <br/>

### 증권사 혹은 거래소
데이터 분석 기술을 개발하면 HTS에서 제공하는 분석기능을 대부분 포함하게 되고, 점차 더 편리한 분석기능이 제공될 것으로 예상합니다. <br/>
개발된 분석플랫폼에 거래기능과 회원관리 기능을 추가하여 사업하게되면 증권사, 혹은 거래소로도 더 발전될 수 있습니다. <br/>
국내 증권사의 경우 시가총액이 수조원이고, 미국 투자은행의 경우 수백조의 시가총액을 형성하고 있습니다. <br/>

<br/>