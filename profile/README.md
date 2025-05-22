# 1. Project Overview
- 프로젝트 이름 : 슥맵
- 기능 : 슥슐랭 가이드(4조 - 김예원, 김혜준), 슥커뮤니티(3조 - 이온유, 조완진)

# 2. Team Members (팀원 및 팀 소개)

|                                          김예원                                           |                                           김혜준                                           |                                          이온유                                           |                                          조완진                                           |
| :---------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------: |
| <img src="https://avatars.githubusercontent.com/u/92143160?v=4" alt="김예원" width="150"> | <img src="https://avatars.githubusercontent.com/u/163358979?v=4" alt="김혜준" width="150"> | <img src="https://avatars.githubusercontent.com/u/212457396?v=4" alt="이온유" width="150"> | <img src="https://avatars.githubusercontent.com/u/73417173?v=4" alt="조완진" width="150"> |
|                                            FE                                             |                                             BE                                             |                                            FE                                             |                                            BE                                             |
|                          [GitHub](https://github.com/yewoniiii)                           |                        [GitHub](https://github.com/mingmingsoo)                         |                        [GitHub](https://github.com/ONYOU-LEE)                         |                        [GitHub](https://github.com/cohenpf)                         |

# 3. Key Features (주요 기능 및 ERD)
- **회원 관리**
  - 회원가입 및 로그인 (계열사, 이름, 연락처 등 관리)
- **맛집 정보 CRUD**
  - 맛집 정보 등록 (상호명, 위치, 가격대 등)
  - 맛집 정보 조회
  - 좋아요 기능
- **커뮤니티**
  - 게시글 CRUD
 
![image](https://github.com/user-attachments/assets/fcbd9677-f93e-4044-941e-895b64665b66)

# 4. Tech Stacks
| Tech Stacks       |                                                                                  |
| ---------- | ------------------------------------------------------------------------------------ |
| FrontEnd     | React, Styled-components                                                                    |
| BackEnd   | Spring Boot                                                   |
| Database    | MySQL                                   |
| API    | Kakaomap API |
| Management     | GitHub, Jira                                                                            |

# 5. Gantt Chart (향후 개발 계획)
- [2025.5.21.] 프로젝트 계획 수립 & 역할 분담
- [2025.5.22. ~ 2025.5.26.] [FE] 화면 설계 & 퍼블리싱 / [BE] API 명세 & 구현
- [2025.5.26. ~ 2025.5.28.] 프론트 - 백 연동 작업
- [2025.5.29. ~ 2025.5.30.] 발표 자료 준비

# 6. Development Workflow (개발 워크플로우)

## Git Conventions

### Commit 규칙

- Commit 메세지
- ex) feat(#10): 검색 결과 필터링 기능 추가

```tsx
git add .
git commit -m "feat(#10): 무엇을 작업"
git push origin 현재 작업 브랜치명
```

| Type       | 의미                                                                                 |
| ---------- | ------------------------------------------------------------------------------------ |
| `Feat`     | 새로운 기능 추가                                                                     |
| `Design`   | 사용자 UI 및 CSS 파일 추가 · 수정                                                    |
| `Chore`    | 패키지 매니저 수정, 그 외 기타 수정 ex) .gitignore                                   |
| `Fix`      | 버그 수정                                                                            |
| `Style`    | 코드의 구조,형식 개선 (코드 formatting, 세미콜론 누락, 코드 자체의 변경이 없는 경우) |
| `Docs`     | 문서 수정                                                                            |
| `Refactor` | 코드 리팩토링                                                                        |
| `Test`     | 테스트 코드, 리팩토링 테스트 코드 추가                                               |
| `Comment`  | comment 필요한 주석 추가 및 변경                                                     |
| `File`     | 파일 또는 폴더명 수정, 이동, 삭제 등의 작업만 수행한 경우                            |
| `!HOTFIX`  | 급하게 치명적인 버그를 고쳐야 하는 경우                                              |

<br/>

### Pull Request 규칙

```
  자주 커밋하고 PR은 300자가 넘지 않도록 주의! (자주 PR)
```

- **develop 브랜치**로 PR 날리기
- PR 제목은 commit 메세지랑 똑같이
  - 제목: **[Feat]** 핵심적인 부분만 간략하게
  - 내용: 간결하게 리스트 방식으로
- merge는 reviewer가 해주기
  : 코드 관련 수정사항, 질문 등 코멘트 남기기

<br/>

### 팀원 리뷰 후 Merge

→ PR 리뷰 시에는 해당 브랜치로 checkout 한 후 확인

→ Approve 이후 Merge 진행

## 브랜치 전략 (Branch Strategy)

### Branch 생성

- **브랜치명**
  : 기능/#이슈번호  
   ex) `feat/#11`, `chore/#5`, `refactor/#8`

```
브랜치 생성 및 이동
git checkout -b 브랜치명
```

- 브랜치 종류
  ### | **branch 종류**
  - `main`: 배포 브랜치
  - `develop`: 개발 브랜치
  - `기능/#이슈번호`: 세부 개발 브랜치

<br/>
