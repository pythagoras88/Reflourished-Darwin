# Changelog

What this fork ([pythagoras88/Reflourished-Darwin](https://github.com/pythagoras88/Reflourished-Darwin)) adds to
[oenderg/Reflourished-Darwin](https://github.com/oenderg/Reflourished-Darwin). The original project's own release
notes are in [release-notes/](release-notes/).

## 2026-10-30

- **Give gems**: adds 100, 1,000 or 10,000 gems once, through the game's own wallet. On iPhone and
  iPad it is a choice in the Settings app that is used when you switch back to the game and then
  resets itself; on the Mac it is a button in Settings > General.
- **The gem multiplier now covers rewards**: quest and Weekly Challenge gems are multiplied too, not
  only gems you collect on the lawn (×10: a 3-gem reward gives 30). A collected gem is still
  multiplied once.

## 2026-10-29

**Cheats**, all off until you turn them on: on iPhone and iPad in the iOS Settings app under
**PvZ2 Reflourished**, on the Mac in Settings > General > Cheats.

- **Unlimited plant food**: once the game has given you plant food in a level, a used one comes back a moment later.
- **Sun multiplier**: ×2, ×3, ×4, ×5, ×10 or ×20 for every sun you collect (×10: 250 instead of 25), up to the level's limit.
- **Coin multiplier**: ×2 to ×10 for every silver, gold and diamond coin you collect on the lawn.
- **Gem multiplier**: ×2 to ×10 for every gem you collect on the lawn.

They go through the game's own code, so the counters, the caps and the collection animations all
agree, and nothing is written into your save directly.

**Fixes**

- Unlimited plant food no longer freezes a new save's first levels. It used to top the counter up as
  soon as a level started; the tutorials decide when you get plant food, and taps stopped working.
  Now it never gives you plant food the game hasn't.

**Changes**

- The app ID is `io.github.pythagoras88.reflourished-modded`, so this build installs beside the original
  (`io.github.oenderg.reflourished-darwin`) as its own app, with its own saves on iPhone and iPad.
- The downloads are named `PvZ2-Reflourished-modded-<game>-Darwin-<version>.ipa` (and
  `-Full.ipa`, `-Mac.dmg`, `-Mac-Full.dmg`).
- The build workflow can build without publishing (the `.ipa` stays on the run's page under
  Artifacts), finds the APK in any draft release, and can use another Mac (`macos-15-intel`) when
  GitHub's Apple silicon Macs are queued.
