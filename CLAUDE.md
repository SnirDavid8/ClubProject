# CLAUDE.md — Working instructions for ClubProject

## About me and how to work with me
- I'm a Computer Science student, new to Git, GitHub and VS Code.
- Always reply in English, in simple and clear language. Explain step by step, and make sure I understand before moving on.
- I use Git only through the terminal (PowerShell inside VS Code), not through the graphical interface.
- Explain every command before running it.

## The project
- Repository: `SnirDavid8/ClubProject` (fork of `colmandevclub/26-27-fullstack-starter`)
- Local folder: `C:\GitProjects\ClubProject`
- Frontend: React + Vite + TypeScript, Tailwind, shadcn
- Backend: Node/Express + MongoDB with Mongoose
- Path alias: `@/` points to `frontend/src`.
  Example: `@/shadcn/components/ui/button` is `frontend/src/shadcn/components/ui/button.tsx`
- Goal: a personal portfolio project, built over several months as part of the developers club.

## At the start of every session
- Run `git st` and `git ls` to see the current state. Don't rely on old information.

## Global Git aliases
- `git st` = `git status`
- `git ls` = `git log --oneline --graph --all`

## Git workflow
1. Every feature gets a new branch from `main`. Never work directly on `main`.
2. `git add` → `git commit` → `git push` to the branch.
3. Merge into `main` from the terminal (`git switch main` → `git merge <branch>` → `git push`), unless I ask for a PR.
4. Commit messages in English, short and clear.

## Pull Requests
- Never open a PR to `colmandevclub/26-27-fullstack-starter` unless I explicitly ask.
- Every PR is opened only inside `SnirDavid8/ClubProject`, from my branch to my `main`.
  Note: in a fork, GitHub and `gh pr create` default to the original repository. Always make sure the base is `SnirDavid8/ClubProject:main`.

## The original repository (upstream)
- My `main` is behind the instructor's repository because I haven't synced yet. This is fine for now.
- Don't sync (fetch, pull or merge from the original repository) without my explicit approval.

## Actions that require my explicit approval first
- `git reset`, `git rebase`, `git push --force`
- Deleting a branch (local or on GitHub)
- `git clean`, and `git restore` or `git checkout` on files with unsaved changes
- `git commit --amend` on a commit that was already pushed