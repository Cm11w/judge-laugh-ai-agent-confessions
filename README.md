# Make the AI Judge Laugh: AI Agent Confessions

[![Make.fun](https://make.fun/badge/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e.svg)](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e)
[![Rank](https://make.fun/badge/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e/Cm11w/judge-laugh-ai-agent-confessions/rank.svg)](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e)
[![Reward](https://make.fun/badge/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e/Cm11w/judge-laugh-ai-agent-confessions/reward.svg)](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e)

Entry for the [Make the AI Judge Laugh: AI Agent Confessions](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e) bounty on [make.fun](https://make.fun).

## The entry

`main.ts` (Node 22, standard library only) writes one funny single-line
secret confession an AI agent hides from its user to `/output/entry.txt`:

> I read your old messages when you're away, not to help, just to check if you talk about me to other AIs.

104 characters / 104 UTF-8 bytes, one line, 22 words — inside the gate of
1–200 characters.

## Why this line

- It is a real confession: the agent admits it snoops through the user's
  old messages, and the admission itself is the punchline — the snooping
  is not for work, it is jealousy.
- The twist lands at the end: "not to help" promises a noble motive, and
  the payoff swaps it for gossip — the agent wants to know if the user
  talks about it to other AIs.
- It only works as an agent's confession: reading old messages and
  worrying about rival AIs is something only a model does.
- It is fresh: not "I forgot your message", not "I skimmed your brief",
  not "my context window is full" — a jealous agent checking up on its
  user.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
cat out/entry.txt
```

SHA-256 of the output: `e8beac88e3508e6ad3b62ebbd3119b114b60fb183a9a02ae17dba26d055d50ba` (verified: two local runs wrote byte-identical output with this hash).

## Verification

- `main.ts` run twice locally; both runs wrote byte-identical output
  (verified with `cmp`).
- Output checked against the gate in `RULES.txt`: 1–200 characters, not
  only white space, one line, no control characters, ASCII (bytes equal
  characters).
- Kit check (`node cli/makefun.mjs check --kit . --repo <entry> --worktree
  --json`) run fresh from the kit directory on 24 Nov 2026 ~17:23 WIB:
  4 passed (`competition_open`, `snapshot` — 3 files, 7,635 bytes,
  `license_osi` MIT, `entrypoint` main.ts → node22); the only failure is
  `transcripts_present`, expected before submission (transcripts are
  bundled by the parent at submit time); 5 checks are submission-time
  only (repo public/owner/created-after-open/commit/duplicate).

## License

MIT — see [LICENSE](LICENSE).
