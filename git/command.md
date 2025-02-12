# 명령어 정리

## `git init`
- 현재 디렉토리에 `.git` 폴더를 생성하여 새로운 git저장소를 초기화

## `git colne` 
- 현재 디렉토리에 원격저장소 폴도에 저장 하는 것 

```
git clone {remote_url}
git clone {remote_url} {directory_name}
```

## 파일의 라이프 사이클 
! [라이프사이클](../assets/lifecycle.png)

tracked: 관리대상임 ,untracked :관리대상이 아님
    - tracked 파일: 이미 스냅샷에 포함돼 있던 파일이다
        -unmodified: 수정하지 않음   modified: 수정함 sateaged(커밋에 저장)



## `git status`
 - 현재 git의 상태 
    tracked untracked 파일이 차이를 가진다 


## `git add`
- working directory에서 변경된 파일을 staginng area에 이동

```
git add {file_name/directory_name}
git add . >> 현재 나의 위치를 기준으로 모든 파일과 폴더 
```

## `git commit`

git에 있는 것을 사진을 찍어서 올리는 것 수정 된 상태가 캡쳐 되어 수정 할 수 없는 상태가 되는 것 

우리는 항상 -m을 사용할 것이고 그 뒤에는 항상 파일명을 적어 둘 것 

## `git log`
- 커밋의 히스토리를 조회 후 q를 치면 터미널 반복에서 빠져나올 수 있삼
- option
    -`--oneline` > 깔금하게 정리해줌
    -`--graph` > 흐름을 보기 좋게 만들어 줌 

## `git remote` 
- 파일명 같은 거라고 하면 될 것 같음
- 원격저장소 관리 명령어

- 원격 저장소 추가하는 명령어
```
git remote add {remote_name} {remote_url}

```
- 원격 저장소 확인 
```
git remote -v
```

-원격저장소 삭제
```
git remote remove {remote_name}
```


` git push origin master or main` >> 파일을 메인에 올렸을 때 사용
` git pull origin master or maim` >>파일을 불러 오던가


## 함께 작업할 경우 

-맥의 경우>> 터미널을 열은 후  `cd Desktop/DAMF2` >> 저장 장소로의 이동이 중요
                        `manis@bagseonmin-ui-MacBookAir DAMF2 % git clone {github 받은 url}`
                         - 그럼 저장 장소에 폴더가 생성 됨 , 굳이 터미널을 통해서 들어갈 필요 없긴 하나, 
                         터미널을 이용 하는 것이 별도의 파일로 생성되어 더욱 편하게 사용 가능

## git branch

- git branch : branch 목록 확인 
- git branch {branch_name}: branch 생성 
- git branch -d {name of file}
