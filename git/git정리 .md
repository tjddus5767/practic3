# Git 정리

**Git = VCS**

Git은 Version Control System이다.

Git Hub는 깃을 이용해 올리는 공간이다.

- Git을 사용할 때 add, commit을 사용함

add는 stage라고 본다. (준비하는 단계), 
commit은 쉽게 생각하면 버전과 같다.

**bash 명령어**

- ls = list item

- cd = change directory
파일 경로를 바꿔준다.
    - cd ~ = 홈 파일 경로로 이동

- pwd = print working directory
현재 파일 경로를 알려줌

- mkdir = make directory

## git 명령어

**git = 버전 관리 툴**

다른 사람과의 협업이 쉽게 가능하다.

**git init = initialize**

-> .git을 만든다. 

- (파일 위치를 확인하고 실행해야 만들어진다.)

**add 파일명.확장자명**
- 파일을 추적하겠다는 뜻이다. 임시 저장 공간에 옮기는 과정이라고 생각하면 쉽다. (Stage Fixeds, 검토)

- add . = 깃 디렉토리 안에 있는 모든 파일을 추적한다.

**commit**
- 복사 붙여넣기와 비슷하다 하지만 엄밀히 따지면 아니다.
    - commit을 하면 저장 공간에 옮기는 과정이다. 

- 버전이라고 볼 수는 없지만 버전의 최소 단위로 볼 수 있다.

- git commit 메세지만 입력하면 커밋 메세지를 입력하는 창이 나온다.

- commit -m 메세지명 = 커밋을 할때 메세지를 남겨 주는 이유는
어떠한 내용인지를 메모하는 것,
메세지를 남겨주지 않으면 커밋을 할 수가 없다.

**log = 깃에 대한 기록을 보겠다.**

**push = 지금까지 커밋 된 파일을 깃허브에 업로드 한다.**

**Repository = git directory를 뜻함**
- remote repository는 github에서 만든 것->
    평상시에 이야기 되는 리포지토리이다.

**checksum**
- git commit을 한 다음 나오는 아이디(?) 같은 것

**checkout**
- commit한 파일(버전)을 확인하는 것
    - branch 개념에서 사용되기 위해 사용됨

- git remote add "name" "url"
>특정 url을 name으로 다루도록 할 수 있게 해준다.

**git push --set-upstream origin master**
> remote 리포지토리를 여러개 만들 수 있기 때문에 내가 어떤 리포지토리에 push를 할지 모른다.

> 그래서, 기본 설정으로 origin위치에 push 해달라고 설정하는 것이다.

**head = 내가 바라보고 있는 branch (commit된 버전id)**
- master를 가르켜서 이동 할 수도 있음 -> checkout master를 입력해 갈 수 있다.

- branch 단위로 움직여야 한다.

github에서 .(마침표)를 누르면 웹 버전의 vscode가 열려서 간단한 코드 수정이 가능하다. (cloud 기반의 vscode)

**pull = github 리포지토리 내에 있는 파일과 폴더를 내가 설정한 파일 위치에 가져온다.**

**clone = 저장소 복제 및 다운로드**
> git clone "url"
- git clone "url" . 을 할 시 .git이 있는 폴더부터 만들어짐

**branch**
- 독립적으로 어떤 작업을 진행하기 위한 개념
    - 커밋 사이를 이동할 수 있는 어떠한 포인터와 같은 것

    - 각각의 브랜치는 다른 브랜치의 영향을 받지 않는다.

 > 여러 작업을 동시에 수행 가능

>여러 작업을 동시에 실행하다가 오류 발생 또는 충돌을 방지하기 위해 사용

**checkout**

브랜치 사이를 이동하기 위해 많이 사용됨

**merge**

- 브랜치를 합치는 명령어 (ex= git merge onezero)
    -  브랜치를 나눠서 파일 만든 것을 하나의 브랜치로 통일 시킨다.

-  브랜치를 이동한 다음에 merge를 입력 해야한다.