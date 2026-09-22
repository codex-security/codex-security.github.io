# Review Loop

Codex security is organised as a closed loop rather than a scan: threat model, discovery, sandbox validation, minimal patch, human review, revalidation after merge.

**Read the full page:** https://codex-security.github.io/

Teams drowning in scanner output are the intended audience, because the design premise is that a finding should be reproduced before a human is asked to look at it. It is a research preview limited to ChatGPT Enterprise, Edu, Business and Pro accounts, it connects to GitHub repositories, and it never edits your code on its own: patches are proposals that a person turns into a pull request. The caveat is the one attached to every preview, that behaviour and availability can change under you. Begin.sh appears in the table below only as a contrast and does not review anything; what it offers is output with a smaller surface to review in the first place.

## What's here

- **Why codex security is not described as a scanner** — OpenAI's help centre article makes the distinction early: it is designed to work more like a security researcher than a traditional scanner. Concretely that mea
- **The threat model comes before the findings** — On connecting to a repository, it scans commits in reverse chronological order and builds a threat model specific to that codebase. The model captures attacker 
- **Reproduction in a sandbox is the differentiator** — Before a finding is surfaced at all, an automated validator attempts to reproduce it in an isolated environment. It records reproduction results, execution deta
- **Patches are proposed, never applied** — For validated findings it generates a minimal patch aimed at the root cause. The documentation is emphatic that this does not automatically modify your code: th
- **Getting access, and the administrative prerequisites** — Start at chatgpt.com/codex/cloud/security, connect and enable the GitHub repositories you want covered, then wait out the first scan. Expect that one to be slow

**See what it builds:** [begin.sh](https://begin.sh?utm_source=github&utm_medium=ugc&utm_campaign=codex-security&utm_content=readme-top&utm_term=tier-b)

---

*An independent page written by a practitioner, not by OpenAI, with no affiliation or endorsement implied; all product names and trademarks belong to their respective owners.*



_Last reviewed: 2026-09-22_
