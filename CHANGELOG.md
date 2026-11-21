# Changelog

## 1.0.2 - 2026-11-21

### Changed
- The release ZIP no longer includes `docs/` (the documentation and its screenshots are published on the documentation site), halving the package size.
- New version number to resubmit the plugin to the Moodle Marketplace, whose automated tests failed on 1.0.1 for an internal reason.

## 1.0.1 - 2026-11-18

### Changed
- README and documentation point to the repository renamed to `moodle-by-kelsoncm/moodle-tiny_toolbar`.

## 1.0.0 - 2026-10-31

First release as the TinyMCE subplugin `tiny_toolbar` (formerly `local_tinytoolbar`, component `tool_tinycustomizer`, which never changed the editor).

### Added
- Site layout of the TinyMCE toolbar and menus, applied after every plugin has added its buttons.
- Presets: Moodle default (no change), minimal, simple, standard, accessibility and custom.
- Custom layout as JSON (`toolbar` groups, `menubar` and the optional `quickbars` selection toolbar), validated on save and stored normalised.
- Capability `tiny/toolbar:use`: users without it keep the Moodle default.
- Visual toolbar builder that lists the buttons registered on the site, with groups, ordering, drag and drop, menus, selection toolbar and a preview editor.
- Privacy API provider, PHPUnit tests, CI with moodle-plugin-ci (Moodle 4.5 and 5.3, PostgreSQL and MariaDB), documentation in English and Brazilian Portuguese, release by draft and verification.

### Removed
- The old `local_tinytoolbar` code: admin page, iframe preview, database table and external functions.
