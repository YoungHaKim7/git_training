# git tag만들기 잘 정리됨
- https://holjjack.tistory.com/213


```bash
❯ git tag
v0.0.1-2026-04-04


❯ ls
Cargo.lock  Cargo.toml  FIX_HISTORY.md  README.md  src/  tests/


❯ git push -d origin v0.0.1-2026-04-04
To https://github.com/YoungHaKim7/tcal_rs.git
 - [deleted]         v0.0.1-2026-04-04

 
❯ git push
Everything up-to-date


❯ git tag v0.0.3-2026-04-04



❯ git push origin v0.0.3-2026-04-04

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/YoungHaKim7/tcal_rs.git
 * [new tag]         v0.0.3-2026-04-04 -> v0.0.3-2026-04-04


❯ git push -d origin v0.0.2-2026-04-04
To https://github.com/YoungHaKim7/tcal_rs.git
 - [deleted]         v0.0.2-2026-04-04


❯ git push -d origin v0.0.3-2026-04-04
To https://github.com/YoungHaKim7/tcal_rs.git
 - [deleted]         v0.0.3-2026-04-04

```
