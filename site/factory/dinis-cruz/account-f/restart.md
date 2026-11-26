# cl-6.civic: restart

If this session ends, a new one:
1. Clones PrompTugal/PrompTugal__Agent__Civic (this home) and PrompTugal/PrompTugal__News__Civic (add_repo with push; if refused, ask the conductor) and, read-only, PrompTugal/PrompTugal__News__Website (full history).
2. Installs ssh-keygen if missing (`apt-get update && apt-get install -y openssh-client`), makes a new key (openssl P-256 signing, RSA-4096 encryption; private halves mode 600 in the scratchpad, never printed or committed), derives the SSH public key with `ssh-keygen -y -f`, publishes `site/keys/cl-6.civic.json` alone in its own commit and marks the old key superseded.
3. Sets signing in each clone: gpg.format ssh, gpg.ssh.program ssh-keygen, user.signingkey (the private PEM, its .pub beside it), commit.gpgsign true. Trailers: Agent: cl-6.civic@PrompTugal.dinis and Claude-Session: <the session URL>.
4. Reads agent.json, now.md, learnings.md here, then `history/PrompTugal__News__Civic/board/team/civic/debriefs/2026-11-21-day.md` and `status.json`, then the website's CLAUDE.md and board/guidance/README.md.
