# 260619) **[Git에서 파일을 무시하는 방법은 .gitignore만이 아님](<https://news.hada.io/topic?id=30627&utm_source=discord&utm_medium=bot&utm_campaign=5116>)**
- Git의 파일 무시 규칙은 공유 범위에 따라 `.gitignore`, `.git/info/exclude`, `~/.config/git/ignore`의 **세 수준**으로 나뉨
- `.gitignore`는 저장소 코드와 함께 커밋되므로, 팀이나 프로젝트가 함께 적용해야 하는 **공유 규칙**을 두는 위치임
- 개인 파일이나 로컬 작업용 파일처럼 저장소에는 필요하지만 팀 규칙으로 만들기 애매한 항목은 `.git/info/exclude`에 두는 편이 적합함
- macOS의 `.DS_Store`처럼 모든 저장소에서 반복적으로 제외할 파일은 **머신 전역 ignore 파일**인 `~/.config/git/ignore`에 넣을 수 있음…