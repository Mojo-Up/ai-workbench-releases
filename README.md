# AI Workbench releases

The signed installers and packages of **Mojo Up AI Workbench** (the desktop app) and the
**AI Workbench node** (the same agent teams on a machine without a desktop), one GitHub release
per version. The source lives in a private repository; this one exists so that package managers
and people can download every release without an account.

## Install

```bash
winget install MojoUp.AIWorkbench                   # Windows
brew install --cask mojo-up/tap/ai-workbench        # macOS
yay -S ai-workbench-bin                             # Arch Linux (AUR)
winget install MojoUp.AIWorkbench.Node              # the node, Windows
brew install mojo-up/tap/mojoup-node                # the node, macOS or Linux
```

Or download from the [latest release](https://github.com/Mojo-Up/ai-workbench-releases/releases/latest)
or the [Mojo Up portal](https://portal.mojoup.com.au/releases/ai-workbench). Every release carries a
`SHA256SUMS` over its files. Windows builds are signed with Azure Trusted Signing (signer "Mojo Up"),
Mac builds with a Developer ID and notarised by Apple.

Documentation: <https://docs.mojoup.ai>. Release notes: <https://docs.mojoup.ai/release-notes/ai-workbench/>.

## Issues

Something wrong with an install or an update? [Open an issue](https://github.com/Mojo-Up/ai-workbench-releases/issues).
