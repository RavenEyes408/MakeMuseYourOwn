# Changelog

All notable changes to Make Muse Your Own are documented in this file.
The format follows Keep a Changelog, and versions follow semantic
versioning: a new middle number for improvements, a new first number
for changes big enough to alter how a setup runs.

## [1.1.1] — 2026-11-17

### Fixed
- The setup file now carries its own pinned links (itself and the
  progress form) inside the bootstrap, so it stands alone when a
  Muse is handed the file's address directly, with no repository
  page in between.
- The bootstrap adopts an existing Make Muse Your Own folder
  instead of overwriting it: an existing progress file is read and
  continued, never replaced, and the saved setup file is refreshed
  only when the version has changed.
- If the setup chat cannot be created, the bootstrap now says what
  happens instead: the setup runs in the current chat, folder,
  files, and gates unchanged, and the substitution is recorded.
- Reopening an existing setup chat now posts one fresh line of
  state from the progress file, since the original seed is stale
  by then.
- Phase 7's machinery instruction now prefers the platform's own
  scheduling and triggers before custom scripts.
- The backup folder example is a placeholder (`backup-YYYY-MM-DD`)
  rather than a real-looking date.

## [1.1.0] — 2026-11-17

### Added
- The setup now runs in its own side chat, named **Make Muse Your
  Own** — created after the person's yes, seeded with the version,
  the source link, and the location of everything, and reopened
  rather than duplicated on a resume or tune-up. When the setup
  ends, the chat stays on as the configuration chat.
- A workspace folder of the same name holds the setup's papers:
  a saved copy of the setup file — verified complete before it is
  saved, and read locally from then on, so the repository is
  fetched once, at the start — the progress file, and the Phase 0
  backup as a dated subfolder.
- Two standing behaviors, settled in Phase 4 and written into the
  proactivity preferences: thinking aloud is not an instruction,
  and settled decisions are not re-raised as open questions.
- Phase 8 says the training rule out loud at handover — a
  correction given plainly is recorded as a standing rule — and
  plants a tune-up sitting a week or two out.

### Changed
- The introduction now names the bootstrap machinery — the fetch,
  the folder, the saved copies, the chat — before the person
  agrees to begin. Their yes covers exactly those acts; everything
  personal still waits for Phase 0 and its own go gate.
- The conducting Muse reads the whole setup file once, up front,
  in the setup chat (it holds a local copy now), then works phase
  by phase as before.
- Phase 2's voice step is an explicit ask, made after the look is
  set, and uses the platform's voice picker: the person describes
  the kind of voice they want and picks by ear from the matches
  it returns. No voice list is hardcoded anywhere.
- Phase 7 builds recurring tasks machinery-first: watching that
  can be stated as plain rules is done by scripts or triggers,
  and the agent wakes only for judgment.
- Version statements and the README's pinned links now point at
  1.1.0. A setup already running on 1.0.x finishes on the version
  it started, as always.

## [1.0.2] — 2026-11-17

### Removed
- The zip download route is gone — from the README, the release
  notes, and this changelog. A zip was described in 1.0.0 and
  1.0.1 but never actually attached to any release; rather than
  keep promising a package that isn't there, the concept is
  removed entirely. The repository link is the one way in, with
  cloning as the technical alternative. (GitHub's own automatic
  source download on the repository page is GitHub's, and stays
  as it is.)

### Changed
- Version statements and the README's pinned links now point at
  1.0.2. No setup content changed: the nine phases run exactly as
  in 1.0.0 and 1.0.1, and a setup already running on an earlier
  version finishes on that version, as always.

## [1.0.1] — 2026-11-17

### Fixed
- SETUP.md guards against partial reads. Its opening now tells the
  conducting Muse to check it holds the whole file — all nine
  phases, through a new closing line, *End of setup — version
  1.0.1.* — before beginning, and to keep fetching if a read
  arrives in pieces. The README's note to the agent says the same.

### Changed
- Version statements and the README's pinned links now point at
  1.0.1. No setup content changed: the nine phases run exactly as
  in 1.0.0. A setup already running on 1.0.0 finishes on 1.0.0,
  as always.

## [1.0.0] — 2026-10-30

### Added
- Initial public release.
- README that introduces the setup twice over: to the person reading
  it, and to the Muse agent handed its link — with a permission gate
  before anything begins.
- SETUP.md: the full setup, in nine phases. Reality check and feature
  inventory first; a free-form interview with an optional import from
  another assistant; character built in words, in a rendered and
  approved look, and in a chosen voice; memory written from the
  person's own words with imported material reviewed twice; proactivity
  and routing as recorded choices; connections verified live, one at a
  time; side chats seeded with charters; three starter tasks with
  plain approval warnings; and a closing verification, cleanup, and
  handover.
- A backup of the person's existing files, promised at the start,
  taken before anything is changed, restorable if the setup doesn't
  suit them — and three starting modes: first setup, tune-up, and
  fresh start without a reset.
- SETUP_PROGRESS.template.md: the progress form that keeps the
  setup's place across sittings.

Versions before 1.0.0 circulated privately as a paste-only draft.
1.0.0 supersedes it.
