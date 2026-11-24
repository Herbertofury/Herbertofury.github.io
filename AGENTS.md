# Repository instructions

Read `.agents/foundry/AGENTS-adapter.md` for the pinned shared engineering core.
Keep this file and nested instructions project-owned: setup, commands, constraints and acceptance belong here.

## Repository-local website contract

This is the public static Enderloom information and connection-policy site, not the desktop application. Root `index.html`, `style.css`, `privacy.html`, `terms.html` and `.nojekyll` are the current source; no package manager or application build is required. Keep desktop implementation work in Enderloom, not here.

For site edits read `.agents/skills/static-site-acceptance/SKILL.md`. Preserve the existing noindex/nofollow/noarchive intent, accessibility and truthful under-development status. Changes to privacy, permissions or legal claims must reflect verified product behavior and the owner's approved intent, not invented assurances. Do not change account grants or repository visibility as part of documentation maintenance.

## Mandatory pre-release optimization gate

Before finalizing every release, follow the owner-mandated [Athena zero-loss pre-release optimization standard](https://github.com/Herbertofury/Athena/blob/main/guidance/PRE_RELEASE_OPTIMIZATION.md). Evaluate shrink-anything, fast-anything and rust-anything using reviewed pinned tools in isolated worktrees; run applicable passes, compare equivalent complete workloads, keep only independently verified improvements, restore rejected changes, and record per-tool evidence or explicit inapplicability/blockers. Never weaken tests, delete required content, force a Rust rewrite or regress functionality, quality, portability, compatibility, security or protected performance metrics. Data/documentation-only releases and existing native Rust paths require honest applicability decisions, not artificial ports. Existing local and pinned governance requirements remain intact.
