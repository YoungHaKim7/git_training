# Generate new SSH key
- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent


<hr />

# SSH 키 관리

- 커널 빌드 서버에 접속할 때는 비밀번호 대신 공개키 인증을 사용하는 것이 보안과 편의성 모두에서 유리합니다. Ed25519 알고리즘은 현재 가장 권장되는 키 타입입니다.

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
