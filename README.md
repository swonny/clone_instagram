# clone_instagram

21.10.11
- makemigration 시 오류 발생
  🔴 ModuleNotFoundError: No module named 'django.utils.six'
  - python  2.x.x 버전에서 3.8로 업그레이드하면서 django.utils.six 라는 모듈이 사라졌기 때문
    - from django.utils.six -> django.utils 를 지운 뒤, from six ~ 로 수정
    - pip version 21.2.4 이상부터 pip install six 명령어 사용 가능하기 때문에
      pip install --upgrade pip 해준 이후 pip install six
    - __init__.py 파일에서 from django.utils.six 에서 django.utils 삭제

- 댓글 사용을 위한 disqus추가
  
