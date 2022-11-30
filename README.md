# Git BLOG 만들기
### applepie의 블로그를 build한 과정입니다
<br>

1. **내 컴퓨터에 Git 설치하기**
  - 컴퓨터에 Git을 설치하고 CLI로 Git을 사용했습니다
  - 윈도우 터미널을 새롭게 설치하여 Git을 사용했습니다.(Window PowerShell을 터미널에서 쓰니까 글씨가 동글동글한게 이뻐요)
<br><br>

2. **블로그용 repository 만들기**
  - repository 이름은 'user_name.github.io' 형식으로 써서 'HGarim.github.io'으로 지었습니다.
  - 이렇게 생성한 remote repository를 내 컴퓨터로 복사해서 local repository를 만들었습니다.
<br><br>

3. **Jekyll과 Ruby 설치하기**
  - Jekyll과 Ruby를 설치하고 터미널에 "bundle install"과 "bundle exec Jekyll serve"를 입력하면 생기는 사이트를 확인했습니다.(기본 테마인 minima 테마가 적용된 정적 사이트)
<br><br>

4. **블로그에 테마 적용하기**
  - 'Mr.Green'이라는 Jekyll 테마를 다운받아서 압축을 해제한 다음 테마 폴더의 모든 파일들을 local repository로 복사&붙여넣기 했습니다. 이때 같은 이름의 파일은 덮어쓰기 했습니다.
  - 테마 'Mr.Green'의 git 주소에서 readme.md 파일을 읽으면서 적용한 테마를 커스터마이징 했습니다.(이 테마에서는 '\_config.yml' 파일과 'en.yml' 파일을 나의 정보에 맞게 수정함)
<br><br>

5. **블로그에 포스팅하기**
  - '\_posts' 디렉토리에서 테마 'Mr.Green'에서 제공된 sample 포스트들(markdown 형식으로 작성된 파일들)을 삭제했습니다. 그리고 제가 올릴 포스트들을 markdown 형식의 파일로 작성한 뒤 '\_posts' 디렉토리에 저장하여 블로그에 포스팅했습니다.
<br><br>

6. **블로그의 post에 댓글 기능 추가하기**
  - **DISQUS에서 shortname 확인하기**<br>
    : 자신의 웹사이트의 shortname을 확인해야 합니다. 과정은 아래와 같습니다.<br>
      DISQUS에 로그인<br>
      \> GET STARTED 버튼 클릭 <br>
      \> I want to install Disque on my site 버튼 클릭 <br>
      \> Create a new site의 항목 작성 > 스크롤 내려서 Basic 선택 <br>
      \> 스크롤 내려서 I don't see my (중략) with Universal Code 선택 <br>
      \> 스크롤 내려서 Configure 버튼 클릭 <br>
      \> Configure Disqus의 Website URL 항목만 작성(블로그의 주소를 작성, 나의 경우 'https://hgarim.github.io' 입력) 후 Complete Setup 버튼 클릭 <br>
      \> 하단의 Dismiss Setup 버튼 클릭 <br>
      \> 상단의 Edit Settings 버튼 클릭 <br>
      \> 자신의 shortname 확인<br><br>
    
  - **local repository에서 comment와 관련된 설정을 하는 코드가 있는 파일 수정하기**)<br>
    : 위의 과정에서 확인한 shortname을 'shortname' 항목에 입력하고 적용한 테마에 따라 추가 설정이 필요하다면 그것도 수정합니다.<br>
      (참고) 보통 '\_config.yml' 파일에 존재하지만 테마마다 조금씩 다를 수 있습니다. 제가 적용한 테마 'Mr.Green'은 'en.yml' 파일과 'posts.yml' 파일을 수정해야 했습니다. 저의 경우 과정은 아래와 같습니다.<br>
      DISQUS 사이트에서 확인한 shortname을 'en.yml' 파일의 disqus_shortname 항목에 입력<br>
      \> 'posts.yml' 파일의 comments 항목의 disqus 항목의 enable 항목에 입력되어있는 false를 true로 수정<br><br>

7. **사이트에 favicon 추가하기**
  - 테마 'Mr.Green'에 기본으로 있었던 'favicons' 디렉토리의 파일들을 삭제하고, 무료 favicon을 다운받아서 'favicons' 디렉토리에 넣었습니다.
