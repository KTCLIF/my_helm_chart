 
## 나만의 helm chart 를 만들고 github pages 로 배포 해보자 

<img src="./assets/image01.png">

### templates yaml 파일 작성법

<img src="./assets/image02.png">

### 작성한 chart 가 잘 실행되는지 확인해 보자

<img src="./assets/image03.png">


### 작성한 helm chart 소스 코드를 일단 github 에 push 한다

```bash
git init
git add .
git commit -m "helm01_member 파일 추가함"
git remote add origin git@github.com:oli999/my-helm-chart.git

### docs 폴더를 구성한다.

```bash

mkdir -p docs
# 우리가 만든 chart를 압축해서 docs/  폴더 안에 저장
helm package charts/helm01_member -d docs/

```