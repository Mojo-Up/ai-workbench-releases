# AI Workbench releases

The signed installers and packages of **Mojo Up AI Workbench** (the desktop app) and the
**AI Workbench node** (the same agent teams on a machine without a desktop), one GitHub release
per version. The source lives in a private repository; this one exists so that package managers
and people can download every release without an account.

## Install

```bash
winget install MojoUp.AIWorkbench                   # Windows
brew install --cask mojo-up/tap/ai-workbench        # macOS
winget install MojoUp.AIWorkbench.Node              # the node, Windows
brew install mojo-up/tap/mojoup-node                # the node, macOS or Linux
```

Debian and Ubuntu: an APT repository, served from this repository's `apt` release, keeps both
current with `apt upgrade`:

```bash
sudo install -d -m 755 /etc/apt/keyrings
curl -fsSL https://github.com/Mojo-Up/ai-workbench-releases/releases/download/apt/mojoup-archive-keyring.gpg | sudo tee /etc/apt/keyrings/mojoup-ai-workbench.gpg >/dev/null
echo "deb [signed-by=/etc/apt/keyrings/mojoup-ai-workbench.gpg] https://github.com/Mojo-Up/ai-workbench-releases/releases/download/apt ./" | sudo tee /etc/apt/sources.list.d/mojoup-ai-workbench.list
sudo apt update && sudo apt install mju-ai-workbench-desktop mojoup-node
```

The repository's key is Mojo Up Releases <releases@mojoup.com.au>, fingerprint
`7FB0 67B6 3EDC 5582 1898 CF68 AE80 0EB1 C61A 8037`.

Or download from the [latest release](https://github.com/Mojo-Up/ai-workbench-releases/releases/latest)
or the [Mojo Up portal](https://portal.mojoup.com.au/releases/ai-workbench). Every release carries a
`SHA256SUMS` over its files. Windows builds are signed with Azure Trusted Signing (signer "Mojo Up"),
Mac builds with a Developer ID and notarised by Apple.

AI Workbench is free to use and not open source: see [LICENSE](LICENSE). Mojo Up's services are
under the [terms of service](https://mojoup.ai/terms).

Documentation: <https://docs.mojoup.ai>. Release notes: <https://docs.mojoup.ai/release-notes/ai-workbench/>.

## Issues

Something wrong with an install or an update? [Open an issue](https://github.com/Mojo-Up/ai-workbench-releases/issues).
