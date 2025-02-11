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
`````


##  `git commit`
- staging area에 있는 변경사항을 커밋하여 스냅샷
