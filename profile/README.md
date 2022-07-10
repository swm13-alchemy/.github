## Convention

### Commit Convention

- task 하나 : 하나의 브랜치 = 1 : 1 로 작업을 한다.
- task 의 하위 이슈(하위 작업)가 생길 경우 브랜치는 생성하지 않는다. (미정)
- 커밋 메세지 첫 줄 컨벤션은 다음과 같다.
    - [헤더]커밋 메세지
    - 헤더 종류는 다음과 같다.
        - add: 기능 구현
        - fix: 코드/버그 수정
        - hofix: hotfix 브랜치에서 생성되는 모든 커밋 헤더
        - docs: 문서 작업
        - PR: PR 생성할 때 붙여주는 헤더
        - test : 페어 끼리 git 작업할때, integration test

예시 : [add][PILLUP-104] summary
  
### Branch Convention

- 브랜치 네이밍 컨벤션
    - {branch name}-{work feature}
  
feature branch 네이밍 컨벤션 예시 : PILLUP-104/feat-addBGM
PILLUP-(지라티켓번호)/{branch name}-{work feature}

### Code Review Convention

1. 궁금한 것
   🤔(:thinking:)
2. 제안 (수정 제안)
   🤝 (악수)
3. 칭찬?
   👍 (+1)
   좋아요
4. 논의
   💬 (말풍선)
5. 이게 뭐람(오타, 버그 가능성)
   🤷‍♂️ 🤷‍♀️ (어깨를 으쓱하는 남자, 여자)

## Branch Strategy

### Release branch를 뺀 Git Flow

![branch 전략](https://user-images.githubusercontent.com/68740465/178145203-5078e3e9-e7bb-4aa4-93fd-78fc8e9db7f7.png)

|Branch|목적|
|---|---|
|master|제품 출시|
|develop|다음 버전 개발|
|feature|기능 개발|
|hotfix|출시된 버전 버그 수정|
