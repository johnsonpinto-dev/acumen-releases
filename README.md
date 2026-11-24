# Acumen releases

Signed installers of Acumen's own programs — **no source code**. Each program has its own release line and
checks only its own:

| Folder | Program |
|---|---|
| `kuzo/` | Kuzo Rope Assessment |

Inside a program's folder, each release line has one `latest.json`:

- `all/` — every installed copy
- `first/` — Acumen's own test machines, before everyone
- `test/` — trials of the update mechanism only, never a version for real work

The installers are files of the GitHub releases of this repository (tag `<program>-<version>`, test line
`<program>-test-<version>`), each with a `.sig` file: the program accepts an update only when that signature
matches the Acumen update key built into it and names the version announced. A version on a line's
`withdrawn` list is flagged in the program until it is updated.

Installing the first time is done by hand; later versions are offered by the program itself and installed
only when the user clicks Install. Using the programs needs a licence from Acumen.
