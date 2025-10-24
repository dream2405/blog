---
slug: git-cheatsheet
title: 깃/깃허브 치트시트
authors: [dream2405]
tags: [git, github, cheatsheet]
image: "./image.png"
draft: true
---

![banner](image.png)

<!-- truncate -->

## Git Config

설정 파일 우선순위

1. `.git/config`: 특정 저장소에만 적용
    - `git config --local` 옵션 (기본값)
2. `~/.gitconfig`, `~/.config/git/config`: 특정 사용자에게만 적용
    - `git config --global` 옵션
3. `/etc/gitconfig`: 시스템의 모든 사용자와 모든 저장소에 적용
    - `git config --system` 옵션 (관리자 권한 필요)

유용한 옵션

- 옵션
    - `git config --global user.name "Jaehyun Nam"`
    - `git config --global user.email namjh@dankook.ac.kr`
    - `git config --global core.editor emacs`
- 설정 확인
    - `git config --list`

## 로컬 저장소 생성

명령어

- `git init`: 로컬 저장소 생성
    - 해당 폴더에 `.git` 디렉토리 생성

## 파일 추가

Staging Area에 파일 추가
- Staging Area는 index라고 하기도 함

명령어

- `git add [파일명]`
- `git add [파일1] [파일2]`
- `git add .`: 현재 디렉토리와 그 하위 모든 변경된 파일들을 한 번에 Staging Area에 추가

