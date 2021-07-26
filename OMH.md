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