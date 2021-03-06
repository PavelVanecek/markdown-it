3.0.0 / 2015-01-04
------------------

- Big split. All "rare" rules moved to external plugins (deflist, abbr, footnote,
  sub, sup, ins, mark).
- Updated CM spec conformance to v0.15 (better unicode support).
- Added `md` (parser instance) link to all state objects (instead of former
  options/parser).
- References/Footnotes/Abbrs moved to `block` chain.
- Input normalization moved to `core` chain.
- Splitted links and images to separate rules.
- Renamed some rules.
- Removed `full` preset. Not needed anymore.
- enable/disable methods now throw by default on invalid rules (exceptions can
  be disabled).
- Fixed inline html comments & cdata parse.
- Replace NULL characters with 0xFFFD instead of strip.
- Removed custom fences sugar (overcomplication).
- Rewritten link components parse helpers.
- More functions in `md.utils`.


2.2.1 / 2014-12-29
------------------

- Added development info.
- Fixed line breaks in definitions lists.
- .use() now pass any number of params to plugins.


2.2.0 / 2014-12-28
------------------

- Updated CM spec conformance to v0.13.
- API docs.
- Added 'zero' preset.
- Fixed several crashes, when some basic rules are disabled
  (block termination check, references check).


2.1.3 / 2014-12-24
------------------

- Added curring to `set`/`configure`/`enable`/`disable` methods.
- Demo rework - now can include plugins.
- Docs update.


2.1.2 / 2014-12-23
------------------

- Exposed helpers into parser instances (for plugins).
- Removed utils from global export - been in instances seems enougth.
- Refactored demo & added markdown-it-emoji to it.


2.1.1 / 2014-12-22
------------------

- Refreshed browser builds, missed in prev release.
- Minor changes.


2.1.0 / 2014-12-21
------------------

- Separated method to enable rules by whitelist (enableOnly).
- Changed second param of enable/disable ruler methods.
- Shortcuts in main class for bulk enable/disable rules.
- ASCII-friendly browserified files.
- Separate package for spec tests.


2.0.0 / 2014-12-20
------------------

- New project name & home! Now it's `markdown-it`,
- Sugar for constructor call - `new` is not mandatory now.
- Renamed presets folder (configs -> presets).
