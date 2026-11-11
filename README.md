# ibyt Language Support for VS Code

Syntax highlighting and navigation for `.ibyt` files.

## Features
- **Hover declarations** – hover a variable, `define`, `enum`, `flag`, enum member, method or a local register variable (`byte $work`) and see its declaration, type and size in bytes. `Module.Name` and `import … aka` aliases work too.
- **Outline** – methods, codeblocks, `->Blocks` and `:Labels`. The outline starts collapsed.
- **Select / copy a whole method** – `Ctrl+Alt+M` selects the method or codeblock around the cursor, `Ctrl+Alt+C` copies it. The same two actions appear as CodeLens above every method and in the editor context menu.

## Install
1. Command line: `code --install-extension ibyt-0.4.0.vsix`, or  
   Extensions view → `...` → *Install from VSIX…*
2. Add the colors from `settings-snippet.json` to your `settings.json`.

## Settings
| Setting | Default | Meaning |
|---|---|---|
| `ibyt.codeLens` | `true` | "Select / Copy" above every method |
| `ibyt.outlineClick` | `off` | `selectMethod`: clicking a method in the Outline selects it completely |
| `outline.collapseItems` | `alwaysCollapse` (set by the extension) | Outline starts collapsed. Applies to all languages; set `"alwaysExpand"` in your settings to undo. |
