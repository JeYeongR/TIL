## 220914-start-git.md

` git & github`

## Shell은 무엇인가?

- 운영체제의 커널과 사용자를 이어주는 소프트웨어

## Shell의 종류

- sh(Bourne Shell)
- csh
- bash
- zsh

## Shell의 커맨드

- pwd : 유저이름
- ls : 디렉토리의 내용보기
- cd (이름) : (이름)디렉토리로 이동
- mkdir (이름) : (이름)의 디렉토리 생성
- touch (이름) : (이름)의 파일 생성
- rm (이름) : (이름)의 파일 삭제
- mv (이름) (위치) : (이름)을 (위치)로 이동
- vi (이름) : Vim
- cat (이름) : (이름)의 내용 출력

## Vim의 커맨드

- h, j, k, l : 왼쪽, 아래, 위, 오른쪽
- i : insert mode
- v : visual mode
- : : command mode
- ESC : normal mode로 돌아감
- d : 삭제
- dd : 라인 삭제
- y : 복사
- yy : 라인 복사
- p : 붙여넣기
- u : 되돌리기

## Command mode의 커맨드

- q : 나가기
- q! : 변화 저장없이 나가기
- w : 저장
- wq : 저장하고 나가기

## git의 특징

- 빠른속도, 단순한 구조
- 분산형 저장소 지원
- 비선형적 개발(수천개의 브랜치) 가능

## git과 github의 차이점

- git : 오픈 소스 버전 관리 시스템
- github : git repository를 위한 웹 기반 호스팅 서비

## git 환경설정

```
$ git config --global user.name "유저네임"
$ git config --global user.email "이메일주소"
$ git config --global core.editor "vim"
$ git config --global core,pager "cat"
```

- 정상 설정 확인
`$ git config --list`


