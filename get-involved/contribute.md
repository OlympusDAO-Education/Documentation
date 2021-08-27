# 기여하기

올림푸스는 자율적으로 운영되므로, 누구나 이 깃북 가이드에 기여할 수 있습니다. 이 페이지에서는 대략적인 작업 참여에 대해 알아봅니다.

## 커뮤니티에 참여하세요 <a id="join-our-community"></a>

[DAO 디스코드](https://discord.com/invite/42xFV68uEf)에 접속해 온보딩 양식을 채워주세요. content creation 파트에 관심을 표시해 주시면, 알맞는 역할을 얻게 될 것입니다. 이후, 컨텐츠 팀의 다른 멤버들과 함께 협업해서 이 문서를 같이 개선해 나가면 됩니다.

_알림: 온보딩 프로세스는 이후 변동이 있을 수 있습니다. 하지만 디스코드에서 멤버들에게 문의하면 커뮤니티가 친절하게 알려드릴 테니 걱정 마세요._ 

## 기 순서 <a id="contributor-workflow"></a>

필수 조건: 교육 팀의 [작업 조직](https://github.com/OlympusDAO-Education)에 반드시 참여해야 합니다. 어떻게 하는지 모르겠다면, [DAO 디스코드](https://discord.com/invite/42xFV68uEf) 참여해 질문해 주세요.

모든 기여자들은 문서가 업데이트 될 때마다 아래 순서를 따라야 합니다. 대략 다음과 같습니다:

1. 깃헙\(GitHub\) 리파지토리를 로컬 저장소에 복사\(Clone\) 하세요.
2. 로컬 개발 브랜치를 생성합니다.
3. 당신의 브랜치를 리파지토리에 푸시\(push\) 합니다.
4. 로컬 브랜치에서 작업을 수행합니다.
5. 변경점을 커밋\(commit\)하고, 작업을 진행하면서 리모트 브랜치에 정기적으로 푸시합니다.
6. 개발이 완성되면, 깃헙에 풀 리퀘스트\(pull request\)를 제출합니다.

깃헙이 익숙하지 않다면, 다음 [깃헙 가이드](https://guides.github.com/activities/hello-world/) 를 참고하세요.

### 초기 셋업  <a id="first-time-setup"></a>

1. [OlympusDAO-Education/Documentation](https://github.com/OlympusDAO-Education/Documentation) 의 깃헙 리파지토리를 복사\(clone\) 합니다.

   `git clone git@github.com:OlympusDAO-Education/Documentation.git`

2. 리파지토리를 복사한 프로젝트 폴더로 이동하여, 아래 명령을 입력합니다.

   `git status`

3. 터미널에 다음과 같은 결과가 출력되어야 합니다.

   > On branch master
   >
   > Your branch is up to date with 'origin/master'.
   >
   > nothing to commit, working tree clean

4. 이제 깃헙 리파지토리를 성공적으로 복사했으며, 로컬에서 작업을 수행하시면 됩니다.

### 브랜치 만들기 <a id="create-a-branch"></a>

리파지토리를 복사한 후, 문서 작업을 시작하면 됩니다. 모든 변경점은 공식적인 마스터 브랜치에 합쳐지기 전에 별도의 브랜치로 저장되어야 합니다.

1. `master` 브랜치로 이동하여 리파지토리와 동기화 합니다.

   ```text
    git checkout master git pull
   ```

2. 작업을 하기 위한 새로운 브랜치를 생성합니다. 여기서는 예시로`foo` 라는 이름을 사용하겠습니다.

   ```text
    git checkout -b foo
   ```

3. 리파지토리에 푸시해서, 다른 멤버들이 이 브랜치에 함께 참여할 수 있도록 합니다.

   ```text
    git push -u origin HEAD
   ```

4. 브랜치 셋업이 잘 되었는지 확인하기 위해, 작업 트리 상태를 확인합니다.

   ```text
    git status
   ```

5. 다음과 같은 결과가 출력되어야 합니다.

   > On branch foo
   >
   > Your branch is up to date with 'origin/foo'.
   >
   > nothing to commit, working tree clean

6. 이제 파일 수정을 시작하면 됩니다. 다음 섹션에서는 변경사을 어떻게 커밋\(commit\) 하는지 보여드리겠습니다.

### 변경사 커밋하기 <a id="commit-changes"></a>

문서의 내용이 변화될 때 마다, 커밋\(commit\)을 통해 Git에 기록할 수 있습니다. 또한 변경사항을 리파지토리에 푸시하여, 다른 멤버들로 하여금 어떤 부분이 변경되었는지 확인하도록 합니다. 중요한 것은 리파지토리를 통해 작업을 백업하는 것입니다.

1. `bar` 파일을 수정한 뒤, 커밋을 한다고 가정해 봅시다. 먼저 스테이징\(staging\) 영역에 추가를 해야 합니다.

   ```text
    git add bar
   ```

2. 작업 트리 상태를 체크하세요

   ```text
    git status
   ```

3. 다음과 같은 결과가 출력되어야 합니다.

   > On branch foo
   >
   > Your branch is up to date with 'origin/foo'.
   >
   > Changes to be committed:
   >
   > \(use "git restore --staged ..." to unstage\)
   >
   > modified: bar

4. 스테이징 영역에 수정된 파일이 추가된 후, 커밋합니다.

   ```text
    git commit
   ```

5. 이제 기본 편집기가 열려야 합니다. 변경사항을 간략히 설명하는 메시지를 작성 후, 파일을 저장하고 종료하여 커밋을 완료합니다.

   ​![Your default editor will be opened when you make a commit](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2F3e7de643cda2bbeb2f5d9c1acdf7da37c33f9c1a.png?generation=1623064180992883&alt=media)​

6. 이제 드디어 리파지토리에 커밋을 푸시할 수 있습니다.

   ```text
    git push
   ```

### 풀 리퀘스트\(Pull Request\) <a id="make-a-pull-request"></a>

수정본이 모두 마음에 든다면, 공식적으로 만들기 위해 풀 리퀘스트를 제출합니다.

1. [OlympusDAO documentation GitHub repository](https://github.com/OlympusDAO-Education/Documentation) 로 이동합니다.
2. 작업중인 브랜치를 선택합니다.

   ​![Select your branch](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2Fb00b3f69c2fcd087265d9f644fe7918898884f2b.png?generation=1623076686276361&alt=media)​

3. 브랜치 선택 후, "Pull request" 버튼을 눌러 제출합니다.

   ​![Make a pull request](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2F9ec63c080fdb10de4764107f8335806579d852be.png?generation=1623076686038374&alt=media)​

4. 풀 리퀘스트 페이지에서, 여러분이 수정한 것에 대해 간략한 설명을 남겨주세요.
5. Education 팀이 리뷰할 수 있게 추가하여, 모두가 풀 리퀘스트를 인지할 수 있도록 합니다.
6. 스스로에게 풀 리퀘스트를 지정하고 제출합니다.

   ​![Submit the pull request](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2F923388c7f127885c32d032982c7218e502fc55a9.png?generation=1623076687062053&alt=media)​

### 변경사항 통합하기 <a id="merge-your-changes"></a>

Education 팀이 당신의 풀 리퀘스트를 승인하면, 당신의 변경사항을 마스터 브랜치에 통합할 수 있습니다. 이를 통해 당신의 변경사항이 공식화 됩니다.

1. [풀 리퀘스트 섹션](https://github.com/OlympusDAO-Education/Documentation/pulls) 으로 이동해서 당신의 풀 리퀘스트를 선택합니다.

   ​![Select your pull request](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2F5ed79214bf08733ff827cd20d6a2bba420bb1733.png?generation=1623114324079177&alt=media)​

2. 풀 리퀘스트가 Education 팀에 의해 승인된 이후 "Squash and merge"를 클릭합니다.

   ​![Merge your changes](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2F1abd2fa78de52699eb0a179bb26cba8589481b83.png?generation=1623114324475557&alt=media)​

3. "Confirm squash and merge"를 클릭해서 변경사항을 마스터 브랜치에 최종 통합합니다.

   ​![Finalize the process](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2Fddc57f20f2ee1418293dba8a13c17f97c4f26fb1.png?generation=1623114322427474&alt=media)

