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


## 성식 주제 : CLI 환경에서 자주 쓰는 명령어 모음집
•	git init : git 생성하기
•	git status: 현재 git 상태를 보여줌, 다음 4가지 상태로 출력
    1)	Untracked files
    2) Changes to be committed
    3) Changes not staged for commit
    4) Nothing to commit, working tree clean
•	git log: 히스토리를 조회하는 명령어, 커밋 단위로 히스토리가 쌓임, log를 볼 줄 알아야 develop, release, hotfix 브랜치가 난무할 때 merge 방향이나 순서를 이해할 수 있음
•	git clone git_path : 코드가져오기
•	git checkout branch_name : 브랜치 선택하기
•	git checkout -t remote_path/branch_name : 원격 브랜치 선택하기
•	git branch branch_name : 브랜치 생성하기
•	git branch -r : 원격 브랜치 목록보기
•	git branch -a : 로컬 브랜치 목록보기
•	git branch -m branch_name change_branch_name : 브랜치 이름 바꾸기
•	git branch -d branch_name : 브랜치 삭제하기
•	git push remote_name — delete branch_name : 원격 브랜치 삭제하기 ( git push origin — delete gh-pages )
•	git add file_path : 수정한 코드 선택하기 ( git add * )
•	git commit -m “commit_description” : 선택한 코드 설명 적기 ( git commit -m “내용”)
•	git commit -a : modified 상태의 파일들에 대해 add와 commit을 동시에 진행함
•	git commit -am : -a와 -m을 합친 것.
•	git commit -amend : 마지막 커밋을 수정할 수 있는 옵션. 현재 stage 상태의 파일들이 마지막 커밋과 합쳐서 다시 커밋 됨.
•	git push romote_name branch_name : add하고 commit한 코드 git server에 보내기 (git push origin master)
    push -f 옵션: push –force의 단축, 내 로컬 브랜치로 원격 브랜치를 강제로 덮어 씌움
    push –set-upstream 옵션: 
•   git push --set-upstream [원격 저장소 이름] [브랜치 이름]
    push 시 fatal: The current branch ... has no upstream branch 에러가 발생할 수 있는데, 이는 원격 저장소에 push하려는 브랜치가 없다는 메시지이다.
이럴 때는 push --set-upstream 옵션을 사용해서 원격 저장소 이름과 브랜치 이름을 명시하면 정상적으로 push된다.
•	git pull : git서버에서 최신 코드 받아와 merge 하기
•	git fetch : git서버에서 최신 코드 받아오기
•	git reset — hard HEAD^ : commit한 이전 코드 취소하기
•	git reset — soft HEAD^ : 코드는 살리고 commit만 취소하기
•	git reset — merge : merge 취소하기
•	git reset — hard HEAD && git pull : git 코드 강제로 모두 받아오기
•	git config — global user.name “user_name ” : git 계정Name 변경하기
•	git config — global user.email “user_email” : git 계정Mail변경하기
•	git stash / git stash save “description” : 작업코드 임시저장하고 브랜치 바꾸기
•	git stash pop : 마지막으로 임시저장한 작업코드 가져오기
•	git branch — set-upstream-to=remote_path/branch_name : git pull no tracking info 에러해결


## 성민 주제 : 체리픽 리뷰
### Git 체리픽(cherry-pick)
목적: 원하는 브랜치에 해당하는 커밋 내용만 반영, 업데이트 할 수 있음.<br/>
예시: branchA에서 커밋한 내용 중 커밋 하나만 branchB에 반영하고 싶은 경우가 체리픽 사용에 좋은 예<br/>
git cherry-pick --<커밋넘버>

### 언제 cherry-pick을 사용?
 - 아직 기존의 Pull Request가 머지가 안된 경우 체리픽을 사용하여 현재 브랜치에 반영한 뒤 계속해서 필요한 작업을 이어나갈 수 있음.
 - 만약 체리픽을 사용하지 않는다면 complict가 발생되기 때문임.

### 체리픽 옵션 알아보기
git cherry-pick --continue : 체리픽이 conflict등으로 실패하는 경우, 계속해서 해결하기 위한 방법<br/>
git cherry-pick --quit : 만약 체리픽이 실패하는 경우 더 진행하지 않고 현재 상태를 빠져나오는 방법<br/>
git cherry-pick --abort : 체리픽 이전 상태로 돌리고 체리픽을 취소하는 방법<br/>
<br/>
url : https://webisfree.com/2017-04-11/git%EC%97%90%EC%84%9C-%EC%B2%B4%EB%A6%AC%ED%94%BD%EC%9D%84-%EC%82%AC%EC%9A%A9%ED%95%98%EC%97%AC-%EC%BB%A4%EB%B0%8B(commit)-%ED%95%98%EB%8A%94-%EB%B0%A9%EB%B2%95%EC%9D%80



────────── 실습 내용 흐름 ──────────  
git remote add origin https://GitHub.com/Cat-Hanbbit/iTshirt.git : 로컬저장소에 원격저장소 주소를 알려줌,  
                                                                   [origin] 이란  이름으로 원격 저장소를 추가하라는 것  
git add README.txt 		: README.txt 파일을 커밋.  
git commit -m "개발자 목록 추가"	: README.txt 파일의 커밋에 '개발자 목록 추가'라는 설명을 붙임.  
git push origin master		: 원격저장소에 푸시.  
git pull origin master		: 원격저장소에 새로운 커밋이 있다면 내 로컬저장소로 받아오기.   

