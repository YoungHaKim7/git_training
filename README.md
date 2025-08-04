<p align="center">
  <img width="40px" src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg"></a>
</p>

<hr>

# link
- [github-프로젝트에-기여하기](#github-프로젝트에-기여하기)
- [gitlab--merge-request](#gitlab--merge-request)
- [github-프로젝트-릴리즈-하는-법](#github-프로젝트-릴리즈-하는-법)
- [github보다-보면-read-only로-표시된-경우를-볼-수-있다-그-이유는](#github보다-보면-read-only로-표시된-경우를-볼-수-있다-그-이유는)

<hr>
  
- Git자주 쓰는 기능들
  - [git 기존 git에 덮어씌우기_존재하는 폴더를 git올리기](#git-기존-git에-덮어씌우기_존재하는-폴더를-git올리기) 
  - [gh login할때 브라우져 강제로 띄우는 github홈페이지 주소](#gh로그인-할때-브라우져-강제로-띄우기)
  - [gn-인기-있는-git-설정-옵션들](#gn-인기-있는-git-설정-옵션들)
  - [git-cheat-sheet](#git-cheat-sheet)
  - [gitignore규칙-한글로-잘-정리됨-모든-폴더-하위폴더까지-적용하는것까지](#gitignore규칙-한글로-잘-정리됨-모든-폴더-하위폴더까지-적용하는것까지)
  - [git-diff](#git-diff)
  - [git-status--sb](#git-status--sb)
  - [git-add-다양한-활용법](#git-add-다양한-활용법)
  - [git-pull-vs-fetch--the-modern-coder](#git-pull-vs-fetch--the-modern-coder)
  - [git-submodule-삭제하는법](#git-submodule-삭제하는법)
  - [git-submodule-update &(업데이트 submodule)Updating SDL_샘플](#git-submodule-update)

<hr>

- Tutorial 
  - [Rust개발자를-위한-git사용법-기초지식](#rust개발자를-위한-git사용법-기초지식)
  - [git-처음-만들어서-git연결-](#git-처음-만들어서-git연결-)
  - [gitignore-느낌표-표시가-무슨-의미인지-알아보자](#gitignore-느낌표-표시가-무슨-의미인지-알아보자)
  - [git_training](#git_training)
  - [git-사용법-한글설명](#git-사용법-한글설명)
  - [git-and-github---0-experience-to-professional-in-1-tutorial-part-1--supersimpledev](#git-and-github---0-experience-to-professional-in-1-tutorial-part-1--supersimpledev)
  - [git depth검색하다가 알게 됨_Git 명령어 정리)](http://minsone.github.io/git/git-command-list)
- Youtube Tutorial
  - [4시간_Learn Git - The Full Course | Boot dev](https://youtu.be/rH3zE7VlIMs?si=RGkRcAeeGFX3hSyl)


<hr>

- Gitlab 배우기
  - [gitlab에서-git-배우기](#gitlab에서-git-배우기)
  - [gitlab-publish-배포](#gitlab-publish-배포)


<hr />

# 기본 루틴 Github기준

```bash
# …or create a new repository on the command line

echo "# rust_test_training" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/YoungHaKim7/rust_test_training.git
git push -u origin main



# …or push an existing repository from the command line

git remote add origin https://github.com/YoungHaKim7/rust_test_training.git
git branch -M main
git push -u origin main
```

```bash
$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
Initialized empty Git repository in /home/y/my_project/rust_lang/9999/rust_test_training/.git/


힌트: 초기 브랜치의 이름으로 '마스터'를 사용합니다. 이 기본 브랜치 이름은
힌트: 변경될 수 있습니다. 초기 분기 이름을 모두 사용하도록 구성하려면
힌트: 이 경고를 억제할 새 리포지토리에 대해 다음과 같이 전화하세요:
힌트:
힌트: git config --global init.defaultBranch <name>
힌트:
힌트: '마스터' 대신 일반적으로 선택되는 이름은 '메인', '트렁크', 그리고
힌트: '개발'. 방금 생성된 분기는 이 명령을 통해 이름을 변경할 수 있습니다:
힌트:
힌트: git 브랜치 -m <이름>
```

<hr>

# 250225)Git 코어 개발자는 Git을 어떻게 설정하고 사용할까? (blog.gitbutler.com)
-  by xguru 2일전
- "Pro Git" 저자인 Scott Chacon이 글로벌로 활성화한 몇 가지 Git 설정과 그 이유를 설명
- 설정 중 다수는 실제로 Git 코어 코드베이스를 작업하는 개발자들로부터 배운 것임
- 아래는 Git을 더 좋게 만드는 `~/.gitconfig` 설정
  - https://news.hada.io/topic?id=19441


<hr />

# GitHub 프로젝트에 기여하기[|🔝|](#link)

https://git-scm.com/book/ko/v2/GitHub-GitHub-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%EC%97%90-%EA%B8%B0%EC%97%AC%ED%95%98%EA%B8%B0

- branch 가져오기 https://cjh5414.github.io/get-git-remote-branch/

- How to Earn with Open Source Contributions
  - https://youtu.be/9AkfNuc_SZ4?si=aCrz0PTXOzHQcHHa

<br>

<hr>

# gh로그인 할때 브라우져 강제로 띄우기[|🔝|](#link)
- https://github.com/login/device
- 출처 :
  - https://github.com/cli/cli/issues/5500

<hr>

# rust개발자를 위한 git사용법 기초지식[|🔝|](#link)
- https://rustc-dev-guide.rust-lang.org/git.html#rebasing-and-conflicts


# Git Merge vs Rebase 시각적 설명 | 어떤 것을 사용해야 할까? | ByteMonk[|🔝|](#link)
- https://youtu.be/cjSjlHUmaBU?si=UoLDT7IBM0gvinst

<hr>

# git 처음 만들어서 git연결 [|🔝|](#link)

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

# .gitignore 느낌표 표시가 무슨 의미인지 알아보자[|🔝|](#link)

https://codingdog.tistory.com/entry/gitignore-%ED%8C%8C%EC%9D%BC%EC%97%90-%EC%9E%88%EB%8A%94-%EB%AC%B4%EC%8B%9C-%ED%8C%A8%ED%84%B4%EA%B3%BC-%EB%8A%90%EB%82%8C%ED%91%9C-%ED%8C%A8%ED%84%B4%EC%9D%84-%EA%B0%84%EB%8B%A8%ED%95%98%EA%B2%8C-%EC%95%8C%EC%95%84%EB%B4%85%EC%8B%9C%EB%8B%A4

<hr>

# github 프로젝트 릴리즈 하는 법[|🔝|](#link)

- https://www.lesstif.com/gitbook/github-20774996.html

<hr>

<br>

<hr>

# **[GN⁺: 인기 있는 Git 설정 옵션들](<https://news.hada.io/topic?id=13405&utm_source=discord&utm_medium=bot&utm_campaign=1480>)**[|🔝|](#link)
- https://jvns.ca/blog/2024/02/16/popular-git-config-options/
- `pull.ff only` 또는 `pull.rebase true`  
  - 두 설정 모두 `git pull`을 실행할 때 브랜치가 상위 브랜치와 다를 경우 실수로 병합 커밋을 생성하는 것을 방지하기 위함.  
  - `pull.rebase true`는 매번 `git pull --rebase`를 실행하는 것과 동일.  
  - `pull.ff only`는 매번 `git pull --ff-only`를 실행하...

<hr>


# Git Cheat Sheet[|🔝|](#link)

- https://sapling-scm.com/docs/introduction/git-cheat-sheet/

![Screenshot from 2024-07-13 19-59-31](https://github.com/user-attachments/assets/3c445424-ddd4-43bd-a51a-0c10653797e0)

- https://www.instagram.com/reel/C6GXtAuLhry/?igsh=Zjkxcm9vdHlidjB1

<hr>

# gitignore규칙 한글로 잘 정리됨( 모든 폴더 하위폴더까지 적용하는것까지!!)[|🔝|](#link)

https://nochoco-lee.tistory.com/46

<hr>

# A collection of useful .gitignore templates |🔝|](#link)

- ```.gitignore```세팅 언어별로 다 정리되어 있다. 굿 👍💕🙌

  - https://github.com/github/gitignore/

<hr>

# git_training[|🔝|](#link)

- git tutorial
  - https://git-scm.com/docs/gittutorial

# git 사용법 (한글설명)[|🔝|](#link)

https://youtu.be/ZqhJnaAPokk


# GitLab : Merge Request[|🔝|](#link)

https://youtu.be/XsyY50cn6s8

<hr>

# Git and GitHub - 0 Experience to Professional in 1 Tutorial (Part 1) | SuperSimpleDev[|🔝|](#link)

https://youtu.be/hrTQipWp6co

# Git and GitHub - 0 Experience to Professional in 1 Tutorial (Part 2) | SuperSimpleDev[|🔝|](#link)

https://youtu.be/1ibmWyt8hfw


<hr>

# Complete Git and GitHub Tutorial for Beginners | Apna College[|🔝|](#link)

https://youtu.be/Ez8F0nW6S-w?si=WB0ZbFC18IHuXboi

<hr>


# git diff[|🔝|](#link)

- 변화된 diff를 볼 수 있다. 굿 👍

  - https://youtu.be/2Y8Mltng5uc

# git status -sb[|🔝|](#link)

- git status

  - 이것만 썼는데 뒤에 옵션이 붙는다. 다 찾아보자

- 요약해서 status볼 수 있다.??


# git add 다양한 활용법[|🔝|](#link)

- git add -u 이거 기능 찾아보자

  - 다른 쓸만한 블로그

    - https://www.gitkraken.com/learn/git/git-add

# Git PULL vs FETCH | The Modern Coder[|🔝|](#link)
- https://youtu.be/T13gDBXarj0?si=jKBpw0DL59eeWOQF

    
<br>

<hr>

# GitLab에서 git 배우기[|🔝|](#link)

https://docs.gitlab.com/ee/tutorials/learn_git.html

# GitLab Publish 배포[|🔝|](#link)

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

# Github보다 보면 read-only로 표시된 경우를 볼 수 있다. 그 이유는[|🔝|](#link)
- https://github.com/naver/yobi/issues/432

# git submodule 삭제하는법[|🔝|](#link)

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



# git 기존 git에 덮어씌우기_존재하는 폴더를 git올리기[|🔝|](#link)

```bash
$ git init
  git add README.md
  git commit -m "first commit"
  git branch -M main
  git remote add origin https://github.com/YoungHaKim7/Investment.git
  git push -u origin main
```

# git submodule update[|🔝|](#link)

- https://nochoco-lee.tistory.com/88

- (업데이트 submodule)Updating SDL

- https://github.com/Ravbug/sdl3-sample

- Just update the submodule:

```
cd SDL
git pull
cd ..

cd SDL_ttf
git pull
```
