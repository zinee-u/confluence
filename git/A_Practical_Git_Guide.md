
## A Practical Git Guide
### git commit message
- git commit message 구조와 사례를 소개한다.

### Message 구조
```
type subject
body
footer
```

#### Type: Commit 종류
- feat: 새로운 기능 추가  
- fix: 어떤 오류 해결  
- refactor: Code의 특정 부분 재정렬 (refactoring)  
- test: test와 관련된 모든 것  
- docs: 문서화에 관한 모든 것  
- chore: 정규 Code 유지 보수, Build 수정, 운영 변경이 없는 경우 등  

#### Subject: 제목
- 최대 50 글자  
- 마침표와 특수기호 사용금지  
- 영문 표기 시, 현재시제를 사용  
- 명령어 사용  
- 제목을 본문으로부터 빈 칸 한줄 띄워 구분  

#### Body: 본문
- 무엇(변경 사항)  
- 왜(이유)  
- 한 줄 최대 72글자  
- 72글자 초과시 문단 생성  

#### Footer: 꼬리말
- ISSUE ID 작성  
- Resolves: 관련 commit  
- See also: 참고 사항  

#### 그 외
- 공백오류 불포함  
- 불필요한 구두점 삭제  
- 영어일 경우 제목 행과 문단의 시작마다 대문자

### ex) git commit message

```
Feat Summarize changes in around 50 characters or less

만약에 필요하다면 보다 자세한 설명을 여기에 쓴다. 내용은 72자 내외에서 마무리하는 것을 권장한다. 어떤 맥락에서는 첫번째 줄은 이메일의 제목처럼 취급되고 나머지가 본문으로 간주된다. 빈 칸 한 줄은 본문과 요약문 및 제목을 구분하기 위한 것으로 본문 전체를 생략하지 않은 이상 필수로 있어야 한다; rebase같은 도구들은 이 본문과 요약문 사이에 빈 칸 한 줄이 없으면 혼란스러워하는 경우도 있다.

커밋 메세지는 명령형으로 적자: 예를 들어 "Fix bug"로 적어야지 "Fixed bug"나 "Fixes bug"가 아니다. 이러한 관습은 git merge나 git revert와 같은 명령어에 의해 생성된 커밋 메세지와 일치하게 된다.

추가 문장들은 빈 칸 한 줄 뒤에 따라온다.

- 글머리 기호가 있어도 괜찮다

- 글머리는 통상적으로 하이픈(-)이나 별(*) 기호 뒤에 한 칸 띄우는 것으로 사용되고 문단과 문단 사이에는 빈 칸 한 줄을 띄우는 것으로 사용되지만 그 외 다양한 법이 존재한다

- 들여쓰기를 사용하자

이슈 트래커를 사용한다면 가장 마지막에 레퍼런스 번호를 이런 식으로 적자.

Resolves: #123
See also: #456, #789
```

### 참고자료
>[hashnode| Which commit message convention do you use at work?](https://hashnode.com/post/which-commit-message-convention-do-you-use-at-work-ck3e4jbdd00zyo4s1h7mc7e0g)  

>[github| Git Commit Message Convention](https://github.com/gyoogle/tech-interview-for-developer/blob/master/ETC/Git%20Commit%20Message%20Convention.md)  