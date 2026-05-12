# GitHub Flow
- Git을 사용하는 협업 방식 중 하나.
- 브랜치 단순하게 관리하는 것.
- 복잡하지 않고 빠르게 개발하고 배포할 수 있도록 하며 스타트업이나 웹 서비스 개발에서 많이 사용됨.  
  
[GitHub Flow 공식 문서](https://docs.github.com/ko/get-started/using-github/github-flow?utm_source=chatgpt.com)

## GitHub Flow 기본 과정
1. main 브랜치에서 새로운 브랜치 생성
2. 기능 개발 및 수정 작업하기
3. commit 작성하여 변경사항 저장
4. GitHub에 push하기
5. Pull Request(PR) 생성하기
6. 코드 리뷰 후 main 브랜치에 merge 하기  
--> GitHub Flow 과정 예시 코드
```bash
git checkout -b feature/login
git add .
git commit -m "feat: 로그인 기능 추가"
git push origin feature/login
```

## GitHub Flow 사용 장점
- **Git Flow**는 main, develop, release, hotfix 등 여러 브랜치 사용하기 때문에 **구조 복잡**하고 대규모 프로젝트에 적합함.
- **GitHub Flow**는 main 브랜치 중심으로 동작해 구조 단순, 이해 수월함.
- **GitHub Flow**는 빠른 배포에 적합하고 관리가 쉬움.

--- 

# Commit Convention
- Commit 메시지를 **일정한 규칙**에 맞게 작성하는 방식.  
- 협업 시 어떤 작업을 했는지 쉽게 파악하고 프로젝트 **관리가 쉬움**.  
- 단순히 "수정", "완성", "최종"으로 작성하는 게 아니라 **어떤 작업을 왜 했는지** 명확하게 남기는 것이 핵심.


## Commit의 대표적 타입
- ``feat``: 새로운 기능 추가
```bash
git commit -m "feat: 상품 검색 기능 추가"
```
- ``fix``: 오류 수정
```bash
git commit -m "fix: 로그인 오류 수정"
```
- ``docs``: READEME, markdown 파일 등 문서 수정
```bash
git commit -m "docs: README 파일 수정"
```
- ``style``: 코드 기능 변화 없이 스타일만 변경
```bash
git commit -m "style: 버튼 CSS 스타일 변경"
```
- ``refactor``: 기능 변화 없이 코드 구조 개선
```bash
git commit -m "refactor: 중복 코드 함수로 분리"
```
- ``test``: 테스트 코드 추가 및 수정
```bash
git commit -m "test: 로그인 기능 테스트 코드 추가"
```
- ``chore``: 패키지 설치, 설정 변경 등 기타 작업
```bash
git commit -m "chore: eslint 설정 추가"
```

## Commit Convention 사용 이유
1. commit 목록만 봐도 어떤 작업 이루어져 있는지 알기 쉽다.
```예시)  
feat: 로그인 기능 추가
fix: 회원가입 오류 수정
docs: README 수정
```
2. 협업 시 변경 내용을 빠르게 이해하기 쉽다.
3. 유지 보수 및 버전 관리가 편리하다.  
: 문제 발생시 어떤 commit에서 문제 생겼는지 추적 쉬움
4. 프로젝트 히스토리를 시간 흐름대로 체계적으로 관리할 수 있다.

## 좋은 commit convention 적는 법
1. **짧고 명확하게 작성**: 무슨 작업 했는지 바로 이해할 수 있도록.  
e.x. feat: Navar 컴포넌트 추가
2. **한 commit에는 하나의 작업만 담기**: 기능 추가와 CSS 수정 등을 한 commit에 모두 담는 상황 피하기
3. **영어 타입 + 한국어 설명 조합 많이 사용**

---

# Pull Request 템플릿
Pull Request를 작성할 때 일정한 형식으로 내용을 작성하도록 만드는 템플릿.  
프로젝트 협업 시 작업 내용을 한눈에 파악할 수 있도록 도움.


## Pull Request 템플릿 사용하는 이유
1. 작업 내용 체계적인 정리 가능.
2. 리뷰어가 변경 사항을 쉽게 확인할 수 있음.
3. 협업 효율이 높아짐.
4. 중요한 내용을 빠뜨리지 않을 수 있음.  
  
[GitHub Pull Request 템플릿 공식 문서](https://docs.github.com/ko/communities/using-templates-to-encourage-useful-issues-and-pull-requests?utm_source=chatgpt.com)