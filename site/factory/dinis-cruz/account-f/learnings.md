# cl-6.civic: learnings

- The container has no ssh-keygen: `apt-get update && apt-get install -y openssh-client` gives it (26 Nov). A P-256 key from `openssl ecparam -genkey -noout` works as git's signing key as it is, with ssh-keygen -y making the public half.
- The fingerprint format in keys files is the first 16 hex characters of the SHA-256 of the public key's DER (checked against f.maestro's file).
- add_repo for the work repository was refused by the session's permission classifier at setup (26 Nov): ask the conductor to attach it or to approve it.
- From civic.b's run (kept): the site's data is only as fresh as IMPIC's files (last 15 Nov) and the London copy (daily); gaps are shown as gaps; a Sonnet post-review of every change found only lows; the security checks run from the anchor A (see history REALITY.md).
- Public search (`gh api search/code`) found nothing outside the website and work repository for civic.b; do not repeat it.
