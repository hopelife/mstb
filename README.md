# breif
- moon stock trading bot


# reference
## book
- 파이썬과 리액트를 활용한 주식 자동거래 시스템 구축
- [파이썬과 케라스를 이용한 딥러닝/강화학습 주식투자 (개정판)](http://blog.quantylab.com/pages/rltrader.html)
- [파이썬을 이용한 자동 주식투자 시스템 개발 튜토리얼](http://blog.quantylab.com/systrading.html)


## gut
- [https://github.com/wikibook/stock-trading](https://github.com/wikibook/stock-trading)
- [https://github.com/helloalpaca/QuantBot](https://github.com/helloalpaca/QuantBot)
- [파이썬과 케라스를 이용한 딥러닝/강화학습 주식투자](https://github.com/quantylab/rltrader)

- [파이썬을 이용한 자동 주식투자 시스템 개발 튜토리얼](https://github.com/quantylab/systrader)


# dev environment
- OS: windows10 / OSX
- language: python, nodejs, react
- DB: mongoDB
- editor: visual studio code
- vcs: git, github


# initial setting

## github repository

### remote

- Create a new repository
![github01](./_docs/images/github01.png)
![github02](./_docs/images/github02.png)
![github03](./_docs/images/github03.png)
![github04](./_docs/images/github04.png)

### local

- clone
```
C:\> cd C:\dev\projects
C:\dev\projects\> git clone https://github.com/hopelife/mstb.git
```

## visual studio code
- 
-


# create stock account

## ebest
- [https://m.ebestsec.co.kr/](https://m.ebestsec.co.kr/)
- [https://www.ebestsec.co.kr/](https://www.ebestsec.co.kr/)

### 이베스트 마인 빅데이터 주식앱(개좌개설)
#### 스마트폰
- 이베스트 마인 설치
- 신규 계좌 개설
- 이베스트 마인 > 공인인증서 발급
- 모의투자 신청
![ebest01](./_docs/images/ebest01.jpg)
![ebest02](./_docs/images/ebest02.jpg)
![ebest03](./_docs/images/ebest03.jpg)
![ebest04](./_docs/images/ebest04.jpg)
![ebest05](./_docs/images/ebest05.jpg)
![ebest06](./_docs/images/ebest06.jpg)

#### PC
- 공인인증서 복사(스마트폰 -> PC)
- 공인인증서 로그인
- xingAPI 패키지 설치(C:\eBEST\xingAPI)
- 통합 홈트레이딩시스템(HTS) 설치

### Download Res Files

- open DevCenter
- download res files


## 
```
set CONDA_FORCE_32BIT=1 && conda create --name <가상환경명> <패키지명>

set CONDA_FORCE_32BIT=1 && conda create --name stock-lab python=3.7
```


## unittest
(ml32) C:\dev\projects\mstb> python -m unittest tests.test_agent_ebests


# 공공데이터 수집(p71)

- data.go.kr
- 한국예탁결제원_기업정보서비스


# install mongoDB(p108)
- https://www.mongodb.com/
- https://www.mongodb.com/try/download/community


# install pymongo
```
C:\> cd C:\dev\projects\mstb
C:\dev\projects\mstb> conda activate ml32
(ml32) C:\dev\projects\mstb>pip install pymongo
```

# window scheduler batch file
- C:\dev\projects\mstb\scripts\start_data_collector_1d.bat
```
ECHO ============================
ECHO Conda Activate
@CALL "C:\ProgramData\Anaconda3\Scripts\activate.bat" ml32
ECHO ============================
ECHO Change Directory
cd C:\dev\projects\mstb
ECHO ============================
ECHO Execute Python
python -m stocklab.scheduler.data_collector_1d %*;
```

# python scheduler
```
(ml32) C:\dev\projects\mstb> pip install apscheduler
```


# flask REST API server
```
(ml32) C:\dev\projects\mstb> python -m pip install Flask Flask-Restful flask-cors
```


# react app
```
C:\dev\projects\mstb>mkdir client
C:\dev\projects\mstb>cd client
C:\dev\projects\mstb\client>npx create-react-app stocklab-react
```

# material ui
```
C:\dev\projects\mstb\client\stocklab-react> npm install @material-ui/core @material-ui/icons --save
```

# start react app
```
C:\dev\projects\mstb\client\stocklab-react> npm start
```


# react-sample
```
C:\dev\projects\mstb\client> npx create-react-app react-sample
```

# react-select
```
C:\dev\projects\mstb\client\stocklab-react> npm install react-select --save
C:\dev\projects\mstb\client\stocklab-react> npm install recharts --save
C:\dev\projects\mstb\client\stocklab-react> npm install material-table --save
```