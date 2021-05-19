# Git 주차별 학습 정리

스파르타 Git - 주차별로 학습한 내용을 관리하는 프로젝트이다. 

Table of Contents
-----------------

<!-- vim-markdown-toc GFM -->

* [1주차 학습 정리](#1주차-학습-정리)
  * [12주차 학습 정리](#12주차 학습 정리)
  * [Using git](#using-git)
  * [Using Linux package managers](#using-linux-package-managers)
  * [Windows](#windows)
  * [As Vim plugin](#as-vim-plugin)
* [2주차 학습 정리](#2주차-학습-정리)
  * [Using Homebrew](#using-homebrew)
  * [Using git](#using-git)
  * [Using Linux package managers](#using-linux-package-managers)
  * [Windows](#windows)
  * [As Vim plugin](#as-vim-plugin)
* [3주차 학습 정리](#3주차-학습-정리)
  * [Using Homebrew](#using-homebrew)
  * [Using git](#using-git)
  * [Using Linux package managers](#using-linux-package-managers)
  * [Windows](#windows)
  * [As Vim plugin](#as-vim-plugin)

1주차 학습 정리
------------
12주차 학습 정리
- 개발된 소스를 git 으로 버젼관리를 하고 싶다. 
- 작성된 문서를 git 으로 관리하고 싶다. 
  ( 현재는 네이버의 포스터로 작성하고 있는데 git 이 더 이점이 있을 것 같다.  )

2. 1주차 주요 개념 키워드 적어보기

Q1. Github 은 무엇인가요?
    => 더 이상 이런 파일은 그만! 하나의 파일로도 버전관리를 할 수 있게 도와줘요.
    
Q2. Git 으로 모든 파일의 내용이 자동 비교가 되나요? 
   => 기본 설정으로는 코드(Python, HTML, JavaScript, Java,...) text 파일, markdown파일(text 파일의 일종), CSV 파일 등 이 가능합니다!   
   => 이미지 파일, Word 파일, PDF 파일, 엑셀 파일은 여러가지 설정을 해주어야 가능하답니다. 기본 설정으로 이런 파일들은 파일의 크기가 변했구나! 만 알 수 있어요~         
 
 
Q3. Github 으로 무엇을 할 수 있을까요? 
   => Git 과 Github 은 다릅니다!  Github 은 Git 원격 저장소 + Git 으로 할 수 있는 커뮤니티 기능 서비스입니다. 
   => 즉, Github 은 Git 으로 된 프로젝트 저장 공간을 제공하고, Git 편하게 사용하기 위한 여러가지 부가기능을 가지고 있어요. 
      Git 이 협업할 때 필수! 라고 했었죠? Github 에는 협업하기 위한 기능들을 가지고 있어요. 마치 개발자들의 SNS 같답니다. 
   => Github 외에도 Git 프로젝트 저장소 +  프로젝트 관리하는 기능을 제공하는 곳으로는 대표적으로 Gitlab, 
      bitbucket 등의 서비스가 있어요.
   => 프로젝트 함께 만드는데 참여하는 것 즉 '프로젝트에 기여하기(contribution)' 하기 위한 여러 기능도 제공합니다. 
      이 부분 버그(프로그램 오류,오작동)가 있어요! 
      알리고 프로젝트를 개선시키려면 어떤게 필요할까? 토의할 수도 있어요. 
      
Q4. Git은 버전관리 도구라고 했습니다. commit(커밋) 은 무엇일까?
   => Git 은 commit(커밋) 을 통해 '현재 프로젝트의 상태'을 저장하고 조회합니다.
   => 여러분들이 '파일 저장' 버튼을 누르면 현재 상태의 파일이 저장되는 것처럼 현재 프로젝트의 상태를 저장할 수 있어요. 
      정확히는 snapshot(스냅샷) 즉, 찰칵 사진을 찍는 것, 현재 프로젝트의 전체 상태를 포착하는 거에요. 
   => commit 은 현재 프로젝트의 상태를 저장하는 것이라는 것을 기억하세요! 파일의 어떤 부분이 변경되었는지를 저장하는 것이 아니랍니다
   
3. windows 에서 Git 관리 폴더 설정하기
   1. sourcetree 를 켜고 Create 
   2. 탐색을 누르고 뜨는 화면에서 바탕화면에 만든  kimchi-recipe 클릭하고 '폴더 선택' 버튼을 눌러주세요
   3. 아래처럼 내용이 잘 채워졌다면 '생성을' 눌러주세요
   4. 아래처럼 팝업이 뜨면 예 를 눌러주세요. 놀라지 마세요! 이미 있는 폴더를 git 폴더로 만들 건지 다시 한번 확인하는 것 뿐이에요
   5. 아래처럼 보이면 잘 된 거에요! 
   
4. Windows 에서 삭제하기
   1. + 를 눌러서 New Tab 을 열어주세요. 
   2. 삭제하려는 저장소를 선택한 후 우클릭 - 삭제를 누르면 팝업이 뜹니다.
   3. sourcetree 에서만 안 보이게 하려면 북마크를 제거하세요 를
      컴퓨터에서까지 삭제하려면 디스크에 있는 저장소를 삭제하세요 를 눌러주세요.
   4. 디스크에 있는 저장소를 삭제하세요 를 누르면 내 컴퓨터에서도 삭제가 됩니다!  
      git 설정이 꼬여서 git 설정만 처음부터 해보고 싶은 거라면 다음 단계를 참고!   
      
      
   5. git 설정이 잘 되지 않아서 프로젝트 파일은 현재 상태 그대로 두고, git 설정만 처음부터 되돌리고 싶은 거라면!
      내 컴퓨터 프로젝트 폴더 내 .git 폴더를 지워주면 됩니다. 
      이 경우, git 프로젝트가 아닌 그냥 일반 프로젝트가 되었다고 생각하면 됩니다. 
      다시 git 프로젝트로 만드는 git 초기화(initialize)부터 해주면 되겠죠?   
      
   6. 원격 repo 사용하기 - 개념탑재      
   
Q1.  원격 repo와 로컬 repo 가 뭐예요
   => Git 도 클라우드 서비스로 두 군데의 내용을 동기화한 것처럼 원격 repo와 로컬 repo 를 연결시켜서 내용을 반영시킬 수 있어요. 
      로컬 repo 가 원격 repo 를 연결하는 것을 추적(Tracking, 트랙킹 / branch tracking) 이라고 해요.

   => 로컬 repo 만이 내가 어떤 원격 repo 와 연결되어있는지를 알고 있어요. 
      원격 repo 는 내가 어떤 로컬 repo 와 연결되어있는지 정보를 가지고 있지 않아요. 
      언제나 로컬 repo 를 기준으로 동작을 이해해주세요! 
   => 로컬 repo 를 기준으로 생각하면 되겠죠? 나(로컬 repo)의 내용을 보내주는 거니까 push! 나(로컬 repo)로 내용을 땡겨오는 거니까 pull!  
   => 원격 repo 를 내 컴퓨터에서도 사용할 수 있도록 가져올 수도 있어요. 일종의 초기 다운로드라고 생각하면 됩니다. 
      이걸 clone(클론, 복제) 라고 해요. 
      
5. 원격 repo 사용하기      
   1. tracking- 로컬 repo 와 원격 repo 연결하기
      원격 repo 가 없으므로 Github 에 원격 repo 를 만들고, 내 컴퓨터에 있는 로컬 repo 와 연결시켜볼게요! 
   2. 원격 repo 만들기  
      github 로그인 후 뜨는 페이지에서 초록색 new 버튼을 눌러서 repo를 만들어보겠습니다
      프로젝트 설명 페이지, 라이센스 등 여러 설정을 할 수 있지만 일단은 가장 간단한 형태로 만들어볼게요! 
      
6. Tracking 하기 Github 에 있는 repository 와 내 컴퓨터에 만들어놓은 repository 연결하기     
   1. Windows 에서 설정하기 
      sourcetree 에 들어가서 kimchi-recipe 창에서 설정 버튼을 눌러주세요
      설정창이 뜨면 원격 -  추가를 누르세요.
      원격 이름 : origin 을 적어주세요. origin 은 원격에 연결하는 저장소를 말할 때 일컫는 이름이에요. 
      아하 보통 이렇게 쓰는구나 하고 넘어가시면 됩니다!
      url/ 경로 : 아까 만들어주었던 github 의 주소를 넣어주세요. 
      앞에 설정이 잘 되었다면 아래처럼 보일 꺼에요. 여러분들은 siyoungoh 대신 여러분들 github 이름이 보이겠죠? 
      여기에서 확인 버튼을 누르면 됩니다
   2. 원격 repo Github 에서 없애는 방법
      Github 에 로그인 한 후 repo 페이지로 가서 Setting 을 누릅니다. 
      options 를 선택한 후 맨 마지막으로 스크롤을 내립니다. 
      Danger Zone 에 있는 Delete this repository (이 repository 지우기) 클릭!
      정말로 지울 것인지 확인하는 창이 뜹니다. 절대 복원할 수 없으니 꼭 주의하세요! 
      하단 빈 칸에 user이름/repository명 형식으로 그대로 적어주세요. 
      그런 다음 I understand the consequences, ~ 버튼을 누르면 repo 가 삭제됩니다. 

2주차 학습 정리
------------


3주차 학습 정리
------------

