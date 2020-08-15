# Markdown Shortcuts

![Extension file size in bytes](https://img.shields.io/static/v1?logo=visual-studio-code&label=made%20for&message=VS%20Code&color=0000ff)
![Visual Studio Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/robole.markdown-shortcuts?logo=visual-studio-code&color=ffa500)
![Extension file size in bytes](https://img.shields.io/static/v1?logo=visual-studio-code&label=size&message=14KB&color=008000)
![Visual Studio Marketplace Rating](https://img.shields.io/visual-studio-marketplace/r/robole.markdown-shortcuts?logo=visual-studio-code&color=yellow)
![Built with](https://img.shields.io/static/v1?label=built%20with&message=good%20vibrations&color=violet)

Markdown shortcuts for snippets.

![example](/img/example.gif)

The cool thing about snippets is that they can be setup to behave like a wizard and guide you to different parts of the snippet for convenient editing. 🧙‍♂️

In the example above, when you insert a task list, you are given options to check/uncheck (x or blank) a task item, you can tab to the text description for that item to edit it, and then tab to do the same for the next task item if you wish. If you don't want to edit the snippet at all, or you are done early, just hit `Enter` and the snippet will be finalised. Easy-peasy! 🙌

The snippets are sourced from:
- [VS Code](https://github.com/microsoft/vscode/blob/f74e473238aca7b79c08be761d99a0232838ca4c/extensions/markdown-basics/snippets/markdown.code-snippets):  Built-in snippets for the basic markdown syntax.
- [Markdown Snippets extension](https://marketplace.visualstudio.com/items?itemName=robole.markdown-snippets): Snippets for extended markdown syntax.

The *Markdown Snippets* extension is installed automatically along with this extension. Nothing extra is required from you ever! 🙂

## Shortcuts

| Name                     | Shortcut      | Prefix           | Defined By                  |
|--------------------------|---------------|------------------|-----------------------------|
| Insert bold text         | Ctrl+b        | bold             | Visual Studio Code          |
| Insert code              | Ctrl+m Ctrl+c | code             | Visual Studio Code          |
| Insert fenced code block | Ctrl+m Ctrl+q | fenced codeblock | Visual Studio Code          |
| Insert heading           | Ctrl+m Ctrl+f | heading          | Visual Studio Code          |
| Insert heading level 1   | Ctrl+m Ctrl+1 | heading1         | Markdown Snippets Extension |
| Insert heading level 2   | Ctrl+m Ctrl+2 | heading2         | Markdown Snippets Extension |
| Insert heading level 3   | Ctrl+m Ctrl+3 | heading3         | Markdown Snippets Extension |
| Insert heading level 4   | Ctrl+m Ctrl+4 | heading4         | Markdown Snippets Extension |
| Insert heading level 5   | Ctrl+m Ctrl+5 | heading5         | Markdown Snippets Extension |
| Insert heading level 6   | Ctrl+m Ctrl+6 | heading6         | Markdown Snippets Extension |
| Insert horizontal rule   | Ctrl+m Ctrl+h | horizontal rule  | Visual Studio Code          |
| Insert image             | Ctrl+m Ctrl+i | image            | Visual Studio Code          |
| Insert italic text       | Ctrl+i        | italic           | Visual Studio Code          |
| Insert link              | Ctrl+m Ctrl+l | link             | Visual Studio Code          |
| Insert ordered list      | Ctrl+m Ctrl+o | ordered list     | Visual Studio Code          |
| Insert quoted text       | Ctrl+m Ctrl+q | quote            | Visual Studio Code          |
| Insert strikethrough     | Ctrl+m Ctrl+s | strikethrough    | Markdown Snippets Extension |
| Insert table             | Ctrl+m Ctrl+t | table            | Markdown Snippets Extension |
| Insert task list         | Ctrl+m Ctrl+x | task list        | Markdown Snippets Extension |
| Insert unordered list    | Ctrl+m Ctrl+u | unordered list   | Visual Studio Code          |

None of these shortcuts are used by default in VS Code with the exception of `Ctrl+b`. This shortcut is used to "show the sidebar", if you are not editing a markdown file, it will still do this. This may not be to your liking, you are free to assign a different shortcut for it, or others if you wish!

### Rationale

I chose these particular shortcuts because:
1. '`Ctrl` plus one key' combinations are mostly used already.
1. '`Ctrl+Shift` plus one additional key' combinations are mostly used already.
1. I wanted to find a consistent and predictable pattern, so opted for combinations that have the same opening sequence.
1. I made an exception for "insert bold" and "insert italic" as most text editors have `ctrl+b` and `ctrl+i` as the shortcuts for these actions, so I thought it best to do the same.

### How to change the shortcuts

Unfortunately, VS Code does show enough information for shortcuts to make it easy for differentiation. You need to know the current keybinding to find what you are looking.

![keyboard shortcuts settings](img/settings.png)

If you want to change the shortcuts for the snippets, you can open the keyboard shortcuts settings, you will find the correct set of shortcuts if you search for "insert snippet", it is all the items where the *when* clause has the condition of `editorTextFocus && editorlangId == 'markdown'`.

There is an [open issue](https://github.com/microsoft/vscode/issues/84072) to improve the keyboard shortcuts settings UI.
