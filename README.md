# TodoTable — v1.0.0

A native Android to-do app with a sortable/scrollable table view, a Huawei-style calendar,
and **Moe Assist** - a built-in assistant that turns plain conversation into structured tasks.

This folder contains the signed release APK for this version. No source code is included here;
see the main repository for that.

## What's in this release

- **Home dashboard** - overdue/due-today counts, a "Top Priorities" list that expands when you
  have more than a handful of tasks
- **Tasks table** - every task at a glance, scrollable in both directions, with zebra-striped
  rows, category and status columns, and optional custom columns (including a truncated Notes
  column)
- **Calendar** - month view with a dot under any day that has something due; tap a day to see
  its tasks below, scrollable
- **Categories** (Work / Personal) and an automatically-derived **status** (Overdue / Due soon /
  Upcoming / Completed) - never stored, always accurate
- **Tick to complete** anywhere in the app — greys out and strikes through in place rather than
  disappearing; long-press any task to edit, mark complete/active, or delete
- **Reminders** - a one-off heads-up before the deadline, optional daily reminders on chosen
  weekdays, and a twice-daily (9am/3pm) nag for anything that's gone overdue, until it's resolved
- **Moe Assist** - type or paste a sentence, a whole paragraph, or a direct instruction
  ("add call the dentist to my list, priority 4, it's personal") and Moe pulls out the task name,
  date, priority, and category on its own. Works fully offline; optionally connects to the real
  Claude API if you add your own Anthropic API key in Profile. Full conversation history with
  rename/delete
- **Manage Columns** - add, edit, reorder, and delete custom columns, each with its own per-task
  value entered right in the Add/Edit screen
- **Import/export** your tasks as JSON, and full **dark mode** support throughout

## Installation

This APK is side-loaded, not installed from the Play Store, so Android will ask you to allow it:

1. Download `TodoTable-v1.0.0.apk` from this release onto your Android device.
2. Tap the downloaded file. If prompted, allow installs from this source
   (**Settings → Apps → Special access → Install unknown apps**, enable it for the app you
   downloaded through, e.g. your browser or file manager).
3. Tap **Install**.

You may see a Google Play Protect warning since this isn't a Play Store build — this is expected
for a side-loaded APK and not a sign of a problem with this specific release.

## Requirements

- Android 8.0 (API 26) or newer

## Notes

- All your data is stored locally on your device - nothing is uploaded anywhere, with the one
  exception being Moe Assist's optional Claude API calls, which only happen if you've chosen to
  add your own API key.
- Because this build is self-signed rather than signed through Google Play, updating in place
  requires installing over the same signing key each release - don't switch signing keystores
  between versions if you want in-place updates to work.

## Changelog

- Initial public release.
