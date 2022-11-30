---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_What_is_this
title: "Git & Github"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Jekyll
# multiple category is not supported
category: make my blog
# multiple tag entries are possible
tags: [jekyll, my blog, git]
# thumbnail image for post
img: ":github.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2022-11-30 10:25:30 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-01-01 10:04:30 +0900
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---
<!-- outline-start -->

## Git
<br>

* Git이란?<br><br>
Git은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 스냅샷 스트림 기반의 분산 버전 관리 시스템이다. 또는 이러한 명령어를 가리킨다. 자세한 내용은 [여기서][What-is-Git] 확인할 수 있다.
<br><br><br>
* Git 사용<br><br>
컴퓨터에 Git을 설치하면 사용할 수 있다. 윈도우 운영체제에서의 Git 설치는 [여기서..][DownloadForWindow]


<br><br><br><br>
## Github
<br>

- **Github이란**<br><br>

Ruby on Rails로 작성된 분산 버전 관리 툴인 깃 저장소(Git repository) 호스팅을 지원하는 웹 서비스이다. 이 또한 자세한 내용은 [여기서][What-is-GitHub] 확인할 수 있다.
<br><br><br>
- **Github 사용**<br><br>

처음이라면 [Github 웹사이트][Github]에 회원가입을 하고 로그인을 한 뒤 repository를 생성하자.
repository를 생성했다면 이것을 내 컴퓨터에서도 사용하기 위해서는 내 컴퓨터로 복사해서 local repository로 써야한다.<br><br>
아래 명령어를 터미널에 입력해서 Github 웹 상의 respository(이를 remote repository 또는 원격 저장소라고 부른다.)를 내 컴퓨터로 가져오자.
```bash
$ git clone (your remote repository address)
```

<br>local repository에서 최초 설정을 하지 않았다면 아래와 같이 해주자.
```bash
$ git config --global user.name "yourName"
$ git config --global user.email "yourEmail"
```
<br>local repository에서 변경한 내용을 remote repository에도 반영하려면 add, commit, push 순으로 명령어를 입력하면 된다.<br><br>
```bash
$ git add .
```
이 명령어를 입력하면 모든 변경 파일들을 add 한다.<br><br>
```bash
$ git commit -m "(커밋 메세지 입력)"
```
변경 사항들에 대한 메세지를 커밋 메세지로 입력하고 commit 한다.<br><br>
```bash
$ git push
```
local repository에서 새롭게 생긴 commit들을 remote repository로 올린다.<br><br>
이때 local repository와 remote repository에서 서로 동기화 하기 전에 같은 파일을 수정하면 conflict가 발생하므로 push 하기 전에 pull 해서 동기화 해주면 좋다.
```bash
$ git pull
```


[What-is-Git]: https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F
[What-is-GitHub]: https://git-scm.com/book/en/v2/GitHub-Account-Setup-and-Configuration
[DownloadForWindow]: https://git-scm.com/download/win
[Github]: https://github.com/

<div id="disqus_thread"></div>
<script>
    /**
    *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
    *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables    */
    /*
    var disqus_config = function () {
    this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
    this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://applepie-2.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
