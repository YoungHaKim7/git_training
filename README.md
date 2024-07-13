# GitHub 프로젝트에 기여하기

https://git-scm.com/book/ko/v2/GitHub-GitHub-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%EC%97%90-%EA%B8%B0%EC%97%AC%ED%95%98%EA%B8%B0

- branch 가져오기 https://cjh5414.github.io/get-git-remote-branch/

- How to Earn with Open Source Contributions
  - https://youtu.be/9AkfNuc_SZ4?si=aCrz0PTXOzHQcHHa

<br>

<hr>

# rust개발자를 위한 git사용법 기초지식
- https://rustc-dev-guide.rust-lang.org/git.html#rebasing-and-conflicts


<hr>

# git 처음 만들어서 git연결 

```bash
echo "# Makefile_training" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/YoungHaKim7/Makefile_training.git
git push -u origin main
```

<hr>

# .gitignore 느낌표 표시가 무슨 의미인지 알아보자

https://codingdog.tistory.com/entry/gitignore-%ED%8C%8C%EC%9D%BC%EC%97%90-%EC%9E%88%EB%8A%94-%EB%AC%B4%EC%8B%9C-%ED%8C%A8%ED%84%B4%EA%B3%BC-%EB%8A%90%EB%82%8C%ED%91%9C-%ED%8C%A8%ED%84%B4%EC%9D%84-%EA%B0%84%EB%8B%A8%ED%95%98%EA%B2%8C-%EC%95%8C%EC%95%84%EB%B4%85%EC%8B%9C%EB%8B%A4

<hr>

# github 프로젝트 릴리즈 하는 법

- https://www.lesstif.com/gitbook/github-20774996.html

<hr>

<br>

<hr>

# **[GN⁺: 인기 있는 Git 설정 옵션들](<https://news.hada.io/topic?id=13405&utm_source=discord&utm_medium=bot&utm_campaign=1480>)**
- https://jvns.ca/blog/2024/02/16/popular-git-config-options/
- `pull.ff only` 또는 `pull.rebase true`  
  - 두 설정 모두 `git pull`을 실행할 때 브랜치가 상위 브랜치와 다를 경우 실수로 병합 커밋을 생성하는 것을 방지하기 위함.  
  - `pull.rebase true`는 매번 `git pull --rebase`를 실행하는 것과 동일.  
  - `pull.ff only`는 매번 `git pull --ff-only`를 실행하...

<hr>


# Git Cheat Sheet

- https://sapling-scm.com/docs/introduction/git-cheat-sheet/

![Screenshot from 2024-07-13 19-59-31](https://github.com/user-attachments/assets/3c445424-ddd4-43bd-a51a-0c10653797e0)

- https://www.instagram.com/reel/C6GXtAuLhry/?igsh=Zjkxcm9vdHlidjB1

<hr>

# gitignore규칙 한글로 잘 정리됨( 모든 폴더 하위폴더까지 적용하는것까지!!)

https://nochoco-lee.tistory.com/46

<hr>

# A collection of useful .gitignore templates 

- ```.gitignore```세팅 언어별로 다 정리되어 있다. 굿 👍💕🙌

  - https://github.com/github/gitignore/

<hr>

# git_training

git tutorial https://git-scm.com/docs/gittutorial

# git 사용법 (한글설명)

https://youtu.be/ZqhJnaAPokk


# GitLab : Merge Request

https://youtu.be/XsyY50cn6s8

<hr>

# Git and GitHub - 0 Experience to Professional in 1 Tutorial (Part 1) | SuperSimpleDev

https://youtu.be/hrTQipWp6co

# Git and GitHub - 0 Experience to Professional in 1 Tutorial (Part 2) | SuperSimpleDev

https://youtu.be/1ibmWyt8hfw


<hr>

# Complete Git and GitHub Tutorial for Beginners | Apna College

https://youtu.be/Ez8F0nW6S-w?si=WB0ZbFC18IHuXboi

<hr>


# git diff

- 변화된 diff를 볼 수 있다. 굿 👍

  - https://youtu.be/2Y8Mltng5uc

# git status -sb

- git status

  - 이것만 썼는데 뒤에 옵션이 붙는다. 다 찾아보자

- 요약해서 status볼 수 있다.??


# git add 다양한 활용법

- git add -u 이거 기능 찾아보자

  - 다른 쓸만한 블로그

    - https://www.gitkraken.com/learn/git/git-add
    
<br>

<hr>

# GitLab에서 git 배우기

https://docs.gitlab.com/ee/tutorials/learn_git.html

# GitLab Publish 배포

- Rust로 Gitlab으로 배포하는 방법(How to make use of the GitLab CI for Rust Projects

  - https://dev.to/xfbs/how-to-make-use-of-the-gitlab-ci-for-rust-projects-4j1o
  
    - example https://gitlab.com/xfbs/rust-gitlab-example/

- How to Enable GitLab Pages for GitLab CE and EE

  https://youtu.be/dD8c7WNcc6s

- Gitlab DevSecOps 파이프라인 소개 : CI/CD 에서 보안검사 쉽게하기!

  - https://youtu.be/AQ4WrAWd3E4
  
- gitlab ci examples

    - https://docs.gitlab.com/ee/ci/examples/
  
  
- 성공한 gitlab?? https://gitlab.com/mike-ensor/gitlab-downloader

  - https://mike-ensor.medium.com/release-multi-target-rust-applications-with-gitlab-ci-90136fa10e4c

# Github보다 보면 read-only로 표시된 경우를 볼 수 있다. 그 이유는
- https://github.com/naver/yobi/issues/432

# git submodule 삭제하는법

http://snowdeer.github.io/git/2018/08/01/how-to-remove-git-submodule/



- 먼저 git submodule deinit -f 명령어를 통해서 해당 모듈을 deinit 해줍니다.
```bash
git submodule deinit -f test_app
```

- 그 다음 .git/modules 폴더에 들어가서 해당 폴더를 삭제합니다.

```bash
rm -rf .git/modules/test_app
```

- 마지막으로 git에서 해당 폴더를 제거해주면 됩니다.

```
git rm -f test_app
```

# git submodule update
https://nochoco-lee.tistory.com/88
