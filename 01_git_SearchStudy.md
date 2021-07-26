# < 2021 학회 운영진 7/27 (화) git 스터디 조사 내용 >
 - 스터디 주제 : 깃과 깃허브에 관련된 모든 내용 가능. 혹은 Ch.5와 ch6에 대한 내용
 - 스터디 목적: 깃&깃허브 이해 + 운영진끼리의 간단한 실습 
 - 스터디 목표: 1. 매 스터디시 정해진 진도까지 공부해오기 (7/27까지 ch.5&6, 7/30까지 ch.7,8,9)
                                           ps. 금욜 이후 핸즈온 머신러닝 진도 예정
               2. 매 스터디시 깃과 관련되어 도움이 될 만한 내용 조사해와서 5분 내외 발표하기
               3. 조사내용 푸쉬, 수정이 있을 경우 풀
  - 조사 내용 형식: 자율. 단, 주제와 url은 남길 것.   
  - 지난번 스터디 예시: 민정- 잘 정리된 블로그로 다양한 용도의 브랜치 사용에 대해 소개
                      영진- git의 간략한 역사와 깃에 대한 내용을 직접 velog에 정리후 소개


## 민정 주제 : origin, master, HEAD 차이
### 1. origin
원격 저장소의 이름 <br/>
ex. git remote add origin [url] 형식으로 원격저장소를 추가하거나
git clone을 통해 원격저장소를 복제한다면 자동으로 origin이라는 이름의 원격저장소가 등록됨

### 2. master
현재 local 컴퓨터에 존재하는 커밋의 위치를 가리킴 <br/>
브랜치 중 가장 중심이 되는 기본적인 브랜치를 master 브랜치라고 부름

### 3. HEAD
현재 내가 어떤 작업공간에 있는지를 나타냄 <br/>
ex. 현재 master 브랜치에서 작업을 하고 있다면 HEAD는 master에 있고
feature 브랜치를 만들어줬다면 HEAD는 feature 브랜치에 있게 됨

### 4. origin/master
origin이라는 이름의 원격 저장소 안에 master 브랜치를 의미 <br/>
보통 원격 저장소를 새로 만들면, 자동으로 가장 초기 상태의 원격 저장소 별칭은 origin으로, 초기 상태의 브랜치는 master로 만들어짐

### 5. origin/HEAD
origin 원격 저장소의 '현재' 코드 상태를 의미 <br/>
origin 원격 저장소는 현재 origin/master 브랜치의 상태와 같음

## 예원 주제 :


## 영진 주제 :


## 보혜 주제 :


## 성식 주제 :


## 성민 주제 :



────────── 실습 내용 흐름 ──────────  
git remote add origin https://GitHub.com/Cat-Hanbbit/iTshirt.git : 로컬저장소에 원격저장소 주소를 알려줌,  
                                                                   [origin] 이란  이름으로 원격 저장소를 추가하라는 것  
git add README.txt 		: README.txt 파일을 커밋.  
git commit -m "개발자 목록 추가"	: README.txt 파일의 커밋에 '개발자 목록 추가'라는 설명을 붙임.  
git push origin master		: 원격저장소에 푸시.  
git pull origin master		: 원격저장소에 새로운 커밋이 있다면 내 로컬저장소로 받아오기.   

