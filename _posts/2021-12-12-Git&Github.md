---
layout: post
title: Git&Github 정리
date: 2021-12-12 15:00:00 +0900
categories: jekyll update
---

# Git이란?
- 여러 사람이 한 번에 코드를 관리하기 용이하게 해주는 **분산 버전관리 시스템** 이다.


## Git 저장소에서 파일의 상태
- **Local** 상태와 **Remote** 상태가 있다.
- 다양한 git 명령어를 통해 git을 관리할 수 있다.

## Git Branch
### git branch가 필요한 이유?
코드의 흐름을 분산시켜 효율적인 개발을 가능하게 해준다.


## Git 명령어
- 현재 작업중인 디렉토리를 git 저장소로 지정
user$  `git init`

- 현재 git 상태 확인하기
user$ `git status`

- example.py를 생성(혹은 수정)하고, 이를 commit에 반영하고 싶은 경우
user$ `git add example.py`

- 변경사항이 반영된 new commit 생성
*-m은 commit message를 작성하기 위한 옵션이다.*
user$ `git commit -m "add example.py"`

- commit 기록 확인하기 (Author, Commitor, Date 등)
user$ `git log`

- branch 생성하기
* git branch <branch 이름>을 통해 branch를 생성한다.*
user$ `git branch <branch_name>`

- branch 전환하기
* 현재 작업중인 branch를 전환해준다*
user$ `git checkout <branch_name>`

-branch 병합하기
*현재 작업중인 branch를 원하는 branch에 병합해준다*
user$ `git merge <branch_name>`

- branch 삭제
*git branch -d <branch 이름>을 통해 branch를 삭제한다*
user$ `git branch -d <branch_name>`

#Github
-원격저장소 중 대표적이다.
- Local 저장소를 넘어 Remote 저장소 관리를 용이하게 해준다



