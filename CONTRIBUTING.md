# Contributing to FPS Prototype 1

Thanks for jumping in! Here's how we work together so we don't step on each other's toes.

## Workflow

1. **Check Issues first** — before starting work, look at the [Issues tab](../../issues) to see what's already claimed or planned. Comment on the issue to claim it (or create one if it doesn't exist yet).
2. **Branch off `main`**:
   ```bash
   git checkout main
   git pull
   git checkout -b feature/short-description
   ```
   Branch naming:
   - `feature/...` — new gameplay/features
   - `fix/...` — bug fixes
   - `art/...` — art/asset work
   - `refactor/...` — code cleanup, no behavior change

3. **Commit often, with clear messages**:
   ```
   Add sprint stamina drain to PlayerController
   ```
   not
   ```
   fix stuff
   ```

4. **Open a Pull Request** into `main` when ready:
   - Describe what changed and why
   - Reference the issue it closes (e.g. `Closes #12`)
   - Keep PRs focused — one feature/fix per PR is easier to review than a giant batch

5. **Review** — at least one other person should look it over before merge, if possible. If it's just you and friends, self-merge is fine for small stuff, but try to at least post in the group chat before merging bigger changes.

## Unity-specific tips (important!)

- **Scenes and prefabs are hard to merge.** Two people editing the same scene at the same time will cause conflicts that Git can't auto-resolve. Try to:
  - Split work by scene/prefab where possible
  - Communicate in advance if you're both touching the same scene
  - Use **Prefab Variants** or separate prefabs instead of editing a shared one directly, when you can

- **Never commit `Library/`, `Temp/`, `obj/`, or `.vs/`** — these are local build caches, not source. They're already excluded in the project's `.gitignore` (inside `fps game/`), so this shouldn't come up, but double check before force-adding files if Unity behaves oddly.

- **Set Unity to Force Text serialization** for scenes/prefabs (Edit > Project Settings > Editor > Asset Serialization > Mode: Force Text). This makes diffs and merges much less painful. Do this once as a team so everyone's on the same setting — ideally before anyone starts committing scene changes.

- If the project ever adds large binary assets (textures, audio, models), consider **Git LFS** to keep the repo size sane.

## Code style

_(Fill in once you decide — e.g. PascalCase for public members, camelCase for private fields, one class per file, etc.)_

## Questions

Just ask in the group chat or open a Discussion/Issue — no dumb questions.
