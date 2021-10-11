# clone_instagram

21.10.11
- makemigration 시 오류 발생
  🔴 ModuleNotFoundError: No module named 'django.utils.six'
  - python  2.x.x 버전에서 3.8로 업그레이드하면서 django.utils.six 라는 모듈이 사라졌기 때문
  
