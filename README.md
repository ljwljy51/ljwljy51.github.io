# ljwljy51.github.io

11주차의 내용까지 정상적으로 잘 진행됐었으나, 테마 적용 과정에서 오류가 발생했다(블로그가 깨져서 보이는 오류).
강의 자료를 따라 다시 처음부터 진행을 해도 같은 오류가 계속해서 발생했고, 결국 구글에서 관련 자료를 찾아 처음부터 다시 진행을 했다.

- 테마 적용  
Layon테마를 적용했을 때 오류가 계속 발생해서 plain-white 테마로 적용해 보았다.  
프로필 사진의 경우, 기본 이미지가 있었으나 assets 폴더에 새로운 이미지를 넣고, _config_ 파일에서 이미지 경로를 수정해 새로운 이미지가 보여지도록 했다.  
_config_ 파일에서 title은 Blog_project로, 프로필 이름과 직업을 적는 부분은 새로운 내용으로 수정해주었다.  

- post 작성  
VSC 환경에도 익숙하지 않아 _config_ 파일과 포스트 내용은 메모장에서 작성해주었다.  
post의 경우, _posts_  폴더 내에 Git&Github에 대한 내용을 작성해주었다.  
강의 교안의 내용대로 markdown 문법을 활용해 가독성이 좋아지도록 했다.  
md 파일 제목은 앞에 날짜를 넣어주었고, 파일 내용 첫 부분에도 알맞은 헤더를 넣어주었다.  


- 시행착오  
서버가 돌아가는 와중에 수정사항이 발생해도 반영이 안되는 경우가 있었다. 따라서 수정 결과를 확인하기 위해 매 번 'bundle exec jekyll serve'명령어를 입력해주었다.  
markdown 형식으로 post 작성 시 예상결과와 다르게 나오는 경우가 있었다. 특히 줄바꿈이 안돼서 당황했었는데, space 두 번으로 줄바꿈이 가능하다는 것을 알 수 있었다.  
space 두 번도 인식이 안되는 경우엔 `<br>`을 사용했다. 기울기 적용의 경우에도 정확한 이유를 알지는 못했지만, <> 기호를 포함한 채 기울기 문법을 사용할 경우, 기울기 적용이 안되는 것을 알 수 있었다.
#나 -등의 문법을 활용할 경우, 뒤에 space를 하나씩 넣어주어야 원하는 결과가 나왔다. 붙여 쓸 경우 문법이 적용되지 않았다.

- 댓글기능 구현
강의가 진행된대로 따라하려 했으나, 내가 사용한 plain-white 테마에는 강의에서 진행된 방식대로 댓글기능을 추가하기에는 기본 설정에서 다른 부분이 너무나 많았다.  
따라서 구글링을 했고, https://github.com/samarsault/plainwhite-jekyll 에서 해결방법을 찾을 수 있었다.
_config.yml_  파일에서 plainwhite:부분 밑에 disqus_shortname 부분을 추가해주었다. 그렇게 했더니 별다른 과정 없이 댓글 기능이 생겨버렸었다.
그 상태에서 push했을 때는 댓글기능이 구현되지 않았지만, _posts_ 에서 내가 작성한 파일 헤더 부분에 `comments: true`를 추가해주었더니 댓글기능이 성공적으로 추가되었다.

- favicon 추가  
구글링을 해보니, plainwhite 테마는 favicon을 지원하지 않는다는 것을 알 수 있었다. 댓글기능의 경우, https://github.com/samarsault/plainwhite-jekyll 에서 구현 방법을 알아낼 수 있었지만, favicon에 대한 설명은 없었다. 따라서 구현하지 못했다.

- 블로그 주소
https://ljwljy51.github.io/
