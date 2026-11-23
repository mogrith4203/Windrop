# Windrop shared context

This file is the shared memory between both collaborators and their Claudes. Read it at the start of every session, and update it at the end.

_Last updated: 2026-11-23 by mogrith4203_

## Goal
Send files between devices that AirDrop doesn't cover:
- Mac ↔ Windows
- iPhone ↔ Windows

## Team
| Person | GitHub | Focus |
|---|---|---|
| Mog | @mogrith4203 | TBD |
| (friend) | @TBD | TBD |

## Current state
Repo just created. No code yet. Tech stack not chosen.

## Decisions
_Format: date, decision, reason, who._
- 2026-11-23: Use this GitHub repo (CLAUDE.md + this file) to share context between our separate Claude accounts. Reason: Claude projects can't be shared across accounts. (Mog)

## Open questions
- Which stack? (for example: one cross-platform desktop app for Mac + Windows, plus a native iOS app or a Share Sheet shortcut for iPhone)
- How do devices find each other? (mDNS/Bonjour on the local network, QR code pairing, or both)
- Transfer protocol? (HTTP over LAN, WebRTC, or raw TCP)

## In progress
_Format: what, who, branch._
- (nothing yet)

## Next up
1. Pick the tech stack and discovery method, then record it under Decisions.
2. Split work: who takes the desktop side and who takes the iPhone side.
3. Scaffold the project and fill in build/test commands in CLAUDE.md.

## Done
- 2026-11-23: Repo set up with shared Claude workflow. (Mog)
