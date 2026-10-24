# Provenance and validation

## Palette origin

The original theme was created on October 4, 2026 by mapping Claude Desktop's cached design-token and desktop-frame colors to T3 Code's theme roles. The original source record identifies this public [Claude stylesheet](https://assets-proxy.anthropic.com/claude-ai/v2/assets/v1/c6a992d55-BIeMdhmo.css). That fingerprinted asset may change or disappear over time.

This repository distributes the resulting color-role mapping, not the source stylesheet, fonts, logos, or application code. It is a snapshot of that palette, not a promise to track every later Claude Desktop design change.

The original theme was named **Claude 桌面**, with the ID `claude-desktop`. The published file changes only the display name to **Claude Desktop**. All 57 light-mode colors and 57 dark-mode colors are unchanged. No community theme file was used as the source of this release.

## Verification on October 24, 2026

- Read the installed theme from a copy of the local theme store; the live store was not modified.
- Compared all 114 stored color values with the original file after normalization by T3's own theme engine: no differences.
- Parsed the release JSON with the unmodified `parseThemeFile` implementation from T3 Code **v0.1.1** and **v0.1.2**: both passed.
- Serialized and re-parsed the theme with each version's native functions: both round trips preserved the parsed theme exactly.
- Verified that the shared palette definitions are unchanged between those two versions. Both parsers resolve 61 roles per appearance: the file specifies 57, and four search-highlight roles use T3's defaults.
- Rendered and visually checked the preview artwork in Chromium. Its colors come directly from the release JSON; the interface layout and sample text are illustrative.

The theme was already installed and in use in the maintainer's T3 desktop app. The original October 4 record also reports a successful import and visual check. This release was not freshly imported through the desktop settings UI, and no separate Windows or Linux desktop run was performed.

## Upstream references

- [T3 theme parser, v0.1.1](https://github.com/pingdotgg/t3code/blob/v0.1.1/apps/web/src/themePalette.ts)
- [T3 theme parser, v0.1.2](https://github.com/pingdotgg/t3code/blob/v0.1.2/apps/web/src/themePalette.ts)
- [T3 appearance documentation](https://github.com/pingdotgg/t3code/blob/main/docs/user/appearance.md)

MIT licensing in this repository covers this adaptation, its documentation, and its preview artwork. It does not grant rights to third-party trademarks or product assets.
