# Code Snapshot

Turn selected code into a beautiful image, copied to the clipboard in one keystroke.

- **⌘⇧C**: copies the selection as a PNG, ready to paste into Slack, a PR or a post.
- **⌘⌥⇧S**: opens the **Snapshot studio**, a live preview with every choice beside it, plus **Copy Image** and **Save PNG…**.
- **Right-click** selected code: *Copy as Image* and *Snapshot Studio…*. The palette has *Code Snapshot: Save Selection as Image…* as well.

Without a selection, the whole file is taken.

## The look

- **Code theme**: *Editor* uses your editor's own colours, or pick Midnight, Neon, Ember, Frost, Forest, Paper or Sakura.
- **Background**: nine gradients, the window's own colour, or transparent.
- **Window**: macOS or Windows buttons, or none; the title is the file's name, its path, or nothing.
- Line numbers (the file's real ones), a soft shadow, a fine window edge, and shared indentation trimmed.
- **Watermark**: on by default ("Made with LDE"). Write your own (`@you · yoursite.dev`) or turn it off. It sits as a pill under the window, or in its corner when the padding is tight.
- **Export size**: 1x to 4x, sharp on any screen.

Set it all under **Settings ▸ Tools ▸ Code Snapshot**, which has a live preview. Choices made in the studio are remembered too.

Images are drawn by the plugin with its own fonts (Fira Mono, Inter, Noto Sans Arabic, under the SIL Open Font License), so they look the same on every machine. Arabic text is joined and runs right to left. Nothing leaves your computer.

Needs LDE's plugin API 1.3.
