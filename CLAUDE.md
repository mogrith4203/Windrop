# Windrop: instructions for Claude

Windrop is an AirDrop-style app for sending files between Mac and Windows, and between iPhone and Windows, over the local network.

Two people work on this repo, each with their own Claude account. Claude sessions do not share memory across accounts, so **this repo is the shared memory**. Follow the routine below every session.

## Every session

**At the start**
1. `git checkout main && git pull`
2. Read `docs/CONTEXT.md` (current state, decisions, who is doing what) before doing anything else.
3. Create a branch for your task: `<your-github-login>/<short-task-name>`.
4. In `docs/CONTEXT.md` under "In progress", add a line saying what you are taking, so the other person's Claude doesn't do the same thing.

**At the end** (or before you stop for the day)
1. Update `docs/CONTEXT.md`: move your item from "In progress" to "Done" or leave a note on where you stopped, record any decision you made in "Decisions" with a one-line reason, and adjust "Next up".
2. Commit and push the branch, then open a pull request against `main`.
3. Ask the other person to review the PR. Don't merge your own PR unless it is only a `docs/CONTEXT.md` update.

## Rules
- Never commit directly to `main`.
- Keep PRs small: one task per branch.
- If `docs/CONTEXT.md` conflicts with what you were told in chat, ask your person which is right, then fix the doc.
- If two branches both edited `docs/CONTEXT.md`, keep both people's entries when resolving the merge conflict.
- Never commit secrets, API keys, signing certificates, or `.env` files.
- Write decisions down. Anything that only lives in one person's chat history is invisible to the other.

## Project overview
See `docs/CONTEXT.md` for the current plan and tech choices. Update this section once the stack and folder layout are settled (build commands, test commands, where each platform's code lives).
