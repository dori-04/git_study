GitHub과 Android를 연결하는 방법
=============================
1. android를 진행하는 최상위 폴더에서 git bash를 연다.
2. git init: .git 폴더 생성
3. git add .
4. git commit -m "First Commit"
5. git add remote origin (주소)
6. git pull
git init 
git add remote origin (주소)
git add . 
git commit -m "First Commit"
여기서 바로 git push하면 local과 remote의 내용이 아예 달라서 전달 되지 않는다.
따라서 기존의 히스토리를 먼저 pull해야 되는데, 내 히스토리와의 분기점이 아예 없는 것을 가져오는 것이기 때문에 rebase 방식을 사용한다.

이후에 git push를 사용할 수 있다. 
git push -u를 사용한다면 기본 연결을 지정함으로서 이후에는 git push만으로 원격으로 전달할 수 있다.
































