# Git BLOG 만들기
### applepie의 블로그를 build한 과정입니다
<br>

1. 내 컴퓨터에 Git 설치하기
  - 컴퓨터에 Git을 설치하고 CLI로 Git을 사용했습니다
  - 컴퓨터에 기본으로 있는 명령 프롬프트는 못생겨서 윈도우 터미널을 새롭게 설치하여 Git을 사용했습니다.(Window PowerShell을 터미널에서 쓰니까 글씨가 동글동글한게 이뻐요)
<br><br>

2. 블로그용 repository 만들기
  - repository 이름은 'user_name.github.io' 형식으로 써서 'HGarim.github.io'으로 지었습니다.
  - 이렇게 생성한 remote repository를 내 컴퓨터로 복사해서 local repository를 만들었습니다.
<br><br>

3. Jekyll과 Ruby 설치하기
  - Jekyll과 Ruby를 설치하고 터미널에 "bundle install"과 "bundle exec Jekyll serve"를 입력하면 생기는 사이트를 확인했습니다.(기본 테마인 minima 테마가 적용된 정적 사이트)
<br><br>

4. 블로그에 테마 적용하기
  - 'Mr.Green'이라는 Jekyll 테마를 다운받아서 압축을 해제한 다음 테마 폴더의 모든 파일들을 local repository로 복사&붙여넣기 했습니다. 이때 같은 이름의 파일은 덮어쓰기 했습니다.
  - 테마 'Mr.Green'의 git 주소에서 readme.md 파일을 읽으면서 적용한 테마를 커스터마이징 했습니다.(이 테마에서는 '\_config.yml' 파일과 'en.yml' 파일을 나의 정보에 맞게 수정함)
<br><br>

5. 블로그에 포스팅하기
6. 블로그의 post에 댓글 기능 추가하기
7. 사이트에 favicon 추가하기
  - 무료 favicon을 다운받아서 테마 'Mr
