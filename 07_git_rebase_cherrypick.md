## cherrypick

특정 버전이 생성될 때의 변화를 가져와서 병합하여 새로운 버전을 만든다.



## git cherry-pick [commit id]

[commit id]의 버전이 생성될 때의 변화를 HEAD에 병합하여 새로운 버전을 만든다



## rebase

base를 바꾼다. log를 선형으로 바꾼다.



## git rebase [브랜치 이름]

* HEAD브랜치의 base를 [브랜치 이름]으로 바꾼다.
* [브랜치 이름]의 작업 내용은 유실되지 않고 HEAD브랜치를 이어서 커밋한 것처럼 log가 선형이 되도록 git이 병합해준다.
* HEAD브랜치를 push하기 전에만 rebase가 가능하다
* merge를 통해 병합한 것과 rebase를 통해 병합한 것의 결과는 같아야 한다.



