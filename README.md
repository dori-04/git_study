GitHub과 Android를 연결하는 방법
=============================
1. android를 진행하는 최상위 폴더에서 git bash를 연다.
2. git init: .git 폴더 생성
3. git add .
4. git commit -m "First Commit"
5. git remote add origin (주소): 원격 저장소와 로컬을 연결
6. git pull --rebase origin (branchname): rebase 방식                            
_아니면 git pull origin (branchname) --allow-unrelated-histories: merge 방식_
8. git push -u origin (branchname)
------------------------------------
**그냥 git pull을 진행하게 되면 원격에 있는 README.md파일의 커밋내용이 로컬에 없기 때문에 merge할 수 없다. (기본적으로 merge는 분기점이 있어야 성립된다.) = unrelated histories error**                             

__________________________________________________________
이를 해결하는 3가지 방법이 있다.
1. rebase 방식을 사용해서 원격의 HEAD에 로컬의 커밋을 이어 붙인다.
2. 강제 merge (이걸 사용할 경우 branch구조가 굉장히 특이하다. 한번 해보길)
3. 원격 저장소 리셋 
  1번 방법을 이용하는게 가장 깔끔하고 안전하다.

참고: https://jobc.tistory.com/177





























