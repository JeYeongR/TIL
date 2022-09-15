## 220914-start-git.md

` git & github`

## Shell은 무엇인가?

- 운영체제의 커널과 사용자를 이어주는 소프트웨어

## Shell의 종류

```
sh(Bourne Shell)
csh
bash
zsh
```

## Shell의 커맨드

```
pwd : 유저이름
ls : 디렉토리의 내용보기
cd (이름) : (이름)디렉토리로 이동
mkdir (이름) : (이름)의 디렉토리 생성
touch (이름) : (이름)의 파일 생성
rm (이름) : (이름)의 파일 삭제
mv (이름) (위치) : (이름)을 (위치)로 이동
vi (이름) : Vim
cat (이름) : (이름)의 내용 출력
```

## Vim의 커맨드

```
h, j, k, l : 왼쪽, 아래, 위, 오른쪽
i : insert mode
v : visual mode
: : command mode
ESC : normal mode로 돌아감
d : 삭제
dd : 라인 삭제
y : 복사
yy : 라인 복사
p : 붙여넣기
u : 되돌리기
```

## Command mode의 커맨드

```
q : 나가기
q! : 변화 저장없이 나가기
w : 저장
wq : 저장하고 나가기
```

## git의 특징

- 빠른속도, 단순한 구조
- 분산형 저장소 지원
- 비선형적 개발(수천개의 브랜치) 가능

## git과 github의 차이점

- git : 오픈 소스 버전 관리 시스템
- github : git repository를 위한 웹 기반 호스팅 서비

## git 환경설정

```
git config --global user.name "유저네임"
git config --global user.email "이메일주소"
git config --global core.editor "vim"
git config --global core,pager "cat"
```

- 정상 설정 확인
`$ git config --list`

## git의 명령

```
git clone (복사해온 주소) : git 저장소 복사
git status : 상태 확인
git add (파일이름) : (파일이름)을  추가
git commit : 커밋하기
git push origin main : main branch를 저장소에 푸쉬
```

#### Coventional Commits
- commit의 제목은 commit을 설명하는 하나의 구나 절로 완성
- 띄어쓰기와 앞글자 대문자하기
- prefix 꼭 달기

```
feat : 기능 개발 관련
fix : 오류 개선 혹은 버그 패치
docs : 문서화 작업
test : test 관련
conf : 환경설정 관련
build : 빌드 관련
ci : Continuous Integration 관련
```

## README.md

- 프로젝트와 Repository를 설명하는 책의 표지와 같은 문서
- 나와 동료, 이 repo의 사용자를 위한 문서

## .gitignore

- git이 파일을 추적할 때, 어떤 파일이나 폴더 등을 추적하지 않도록 명시하기 위해 작성
- 해당 문서에 작성된 리스트는 수정사항이 발생해도 git이 무시

## 가장 많이 사용하는 License

- MIT License : MIT에서 만든 라이센스로, 모든 행동에 제약이 없다
- Apache License 2.0 : Apache 재단이 만든 라이센스로, 특허권 관련 내용이 포함
- GNU General Public License v3.0 : 가장 많이 알려져있으며, 의무사항이 존재

## Branch

- 분기정을 생성하여 독립적으로 코드를 변경할 수 있도록 도와주는 모델

```
git branch : 로컬 브랜치 보
git branch (이름) : (이름)의 브랜치 만듬
git switch (이름) : (이름)으로 브랜치 스위치
git merge (이름) : (이름)의 브랜치를 현재 브랜치와 병합
git branch -D (이름) : (이름)의 브랜치를 삭제
git branch origin (이름) : (이름)의 브랜치를 저장소에 푸쉬

#### merge 충돌
- 둘 중 원하는거 선택, 에러는 아님
