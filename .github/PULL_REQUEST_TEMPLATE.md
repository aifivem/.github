<!--
Title: a Conventional Commit, it becomes the release note line.
  feat(<script>): <what players or owners get>    fix(<script>): <what was wrong>    perf: / refactor: / docs: / chore:
Written with an AI? Have it read CLAUDE.md, .claude/rules/ and the script's CLAUDE.md in the aicore-server repo first,
and keep every checkbox below honest.
-->

## What changes

<!-- One or two sentences, from a player's or server owner's point of view. -->

## Why

<!-- The problem it solves. Link the issue: "Closes #123". -->

## How

<!-- The approach in a few lines: files or systems touched, lib helpers used, anything a reviewer should look at first. -->

## Tested

<!-- What you did in game and what you saw (screenshots or a short video help). Say so if it was not tested in game. -->

## Checklist

- [ ] `bun run typecheck`, `bun run lint` and `bun run build` pass, and the build (`dist/`, `fxmanifest.lua`) is committed with the source.
- [ ] The script was restarted and the console showed no `SCRIPT ERROR` or `[client error]`.
- [ ] Uses `@aifivem/lib` and ai-core instead of writing its own helper (`.claude/rules/scripts.md`).
- [ ] Server data reaches clients as one snapshot plus deltas, only to who needs it (no polling, no "refetch" signals).
- [ ] Settings a server owner tunes are in the admin panel, not in a config file; player-facing text is in `locales/en.json`.
- [ ] No version bump by hand: release-please does it from the commit title.
- [ ] Code or ideas taken from another open-source project are credited in `CREDITS.md` of aicore-server.
