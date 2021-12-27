# quiver-fastsearch-alfred
An Alfred workflow that searches Quiver notes by title. Searches run in ~100ms on a collection of 1000 notes.

This workflow just wraps a bash script which uses `ripgrep` to search across note titles in Quiver's json files. **You will need to install ripgrep to use this workflow** (see below). In my testing ripgrep runs about 2x faster than using the standard `grep -R`.

### Download
Download the workflow file on the [releases page](https://github.com/noelcody/quiver-fastsearch-alfred/releases).

### Setup
1. Install [ripgrep](https://github.com/BurntSushi/ripgrep): `brew install rg`

This install command uses homebrew. If you don't have homebrew installed, see the [official homebrew documentation](https://brew.sh/).

The workflow expects rg to install to `/usr/local/bin/rg`. After running homebrew verify the install location with `which rg`.

2. Set your Quiver library directory as the `LIBRARY` value in the workflow's variables (the *`[x]`* at the top-right of the workflow).
