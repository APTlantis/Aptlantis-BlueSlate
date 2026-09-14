# Aptlantis Blue Slate

A dark SiYuan translation of the Aptlantis Blue Slate design system.

Blue Slate uses layered navy neutrals to carry the workspace, reserving saturated colors for interaction, focus, semantic status, graph roles, and editorial meaning. The SiYuan translation gives the toolbar, docks, editor, tabs, menus, databases, and code distinct but related surfaces so the hierarchy remains visible at rest.

## Source Material

- Logo: `blueslate-refs/aptlantis-logo.png`
- Detailed component and state reference: `blueslate-refs/Blue Slate Bootstrap Theme Board.png`
- Web component and Prism-role source: `blueslate-refs/styles.css`
- Additional site captures in `blueslate-refs/`

## Package Files

- `theme.json`: SiYuan package metadata
- `theme.css`: Blue Slate reference tokens, semantic roles, the complete SiYuan 3.8 theme contract, and component styling
- `icon.png`: marketplace icon using the supplied Aptlantis Blue Slate logo
- `preview.png`: compressed 1024 × 768 reference board showing the palette, hierarchy, states, and component language

## Semantic Anchors

- Chassis / void: `#050913`
- Editor / deep: `#0B1728`
- Raised panel / abyss: `#172536`
- Control / navy: `#192E46`
- Border / ridge: `#36485A`
- Primary signal: `#00D8FF`
- Focus signal: `#65F2FF`
- Text / archive: `#E1E7DB`

## Code Highlighting

SiYuan renders fenced code with Highlight.js. Loading the supplied Prism JavaScript would create a competing runtime, so this package instead maps the Blue Slate Prism roles onto SiYuan's native `.hljs-*` classes. The syntax language stays consistent without adding JavaScript or network dependencies.

## Design Rule

Neutrals carry structure. Saturated colors communicate meaning. Blue Slate is a single dark theme and does not introduce a light-mode variant.

## Compatibility

The theme is authored against the SiYuan 3.8.3 theme-variable and selector contract. It uses only `theme.css`; SiYuan's deprecated `theme.js` entry point is not included. When replacing files in an already-running SiYuan workspace, restart SiYuan before visual evaluation because the kernel caches installed theme assets.
