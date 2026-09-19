# Generate new SSH key
- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent


```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

<hr />

# SSH 키 관리

- 커널 빌드 서버에 접속할 때는 비밀번호 대신 공개키 인증을 사용하는 것이 보안과 편의성 모두에서 유리합니다. Ed25519 알고리즘은 현재 가장 권장되는 키 타입입니다.
  - https://www.minzkn.com/linuxkernel/pages/remote-dev.html#ssh-key-management

```bash
# Ed25519 키 생성 (권장)
ssh-keygen -t ed25519 -C "kdev@kernel-build" -f ~/.ssh/id_ed25519
# 공개키를 빌드 서버에 등록
ssh-copy-id -i ~/.ssh/id_ed25519.pub kdev@kernel-build
# ssh-agent 시작 및 키 등록 (~/.bashrc에 추가)
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
# 키 등록 확인
ssh-add -l
```


# git-credential-osxkeychain access key 해결

# Another good HTTPS option 이걸로 해결함

If you want to stay with HTTPS, GitHub currently recommends Git Credential Manager (GCM) or GitHub CLI rather than manually managing PATs. GCM can authenticate through your browser and store the credentials in the macOS Keychain.

For example:

```bash
brew install --cask git-credential-manager

# 인스톨하고
$ git-credential-manager github login
info: please complete authentication in your browser..
```

- https://velog.io/@saichoiblog/macOS-GitHub-push-%EC%8B%9C-git-credential-osxkeychain-%ED%82%A4%EC%B2%B4%EC%9D%B8-%ED%8C%9D%EC%97%85-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0SSH-Key-%EB%93%B1%EB%A1%9D
