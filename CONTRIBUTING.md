# Shaping the extras

Extras are Future Radio characters who keep turning up without a story of their own yet.
Each lives in a folder of their own here (`yuria/`, `the-cat/`): what we know, what we don't know yet, and every appearance.
What you notice about them is how they get a story — and if enough people care about one,
they get promoted to a dressing room of their own, history and all.

## Talk to one

```bash
git clone <this repo> && cd <this repo>
npx github:leo-guinan/future-radio-character-bible chat yuria
```

`/propose <note>` in the chat writes a viewer note into that extra's folder.

## Propose something

- **A viewer note** — `<name>/memory/viewer-notes/YYYY-MM-DD-short-title.md`:

  ```markdown
  ---
  from: your name or handle (or "anonymous")
  experience: what you watched or heard — the episode, the scene, the moment
  episode: E01
  ---
  What should be true about them from now on, in a sentence or two.
  ```

- **An answer to an open question** — edit "What we don't know yet" in their `CHARACTER.md`
  and say where the answer comes from.
- **A new extra** — someone you noticed in an episode who isn't here yet. Open an issue with
  the "New extra" form, or add a folder with a `CHARACTER.md` in the same shape as the others.

No GitHub account? The "Viewer note" issue form works too.

## What can't change in a pull request

- Any extra's `history/` and `history.jsonl` — the writers' room writes those.
- Any extra's `memory/notes.md` is append-only.
- `bible/` folders are generated; leave them out and they're rebuilt on merge.

A check runs on every pull request, once per extra the PR touches, and explains anything it rejects.
