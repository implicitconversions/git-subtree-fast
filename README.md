# git-subtree-fast

A modified version of `git subtree` optimized for use in `subtree --squash` workflows.

If you aren't keen on squash-style subtree workflows, then probably this tool isn't for you.

Includes a command `git-subtree-init` which creates local shell scripts to expedite the
activities associated with subtree add, push, pull, and reset commands.

## Installation

The git subtree tools installer can be downloaded from github via curl:

```
curl -sS -O https://raw.githubusercontent.com/implicitconversions/git-subtree-fast/main/fetch-subtree-tools
```

Install to your PATH using something like this:
> ./fetch-subtree-tools [DEST]

where DEST is a target dir that's in your PATH. Typical examples:"

```
# preferred installation to your HOME dir. Assumes you have ~/bin in your PATH (usually this is set up
# via your `~/.bash_profile`)
./fetch-subtree-tools ~/bin"

# this works well in MSYS2 on Windows. Probably don't do this if using Linux.
./fetch-subtree-tools /usr/bin"
```

Once installed, updating the subtree tools to latest upstream `main` branch can be done at any time by
running the `fetch-subtree-tools` command. It will perform a smart update over itself.

## Usage

### git-subtree-init

_(todo)_

### git-subtree-add

_(todo)_

### git-subtree-pull

_(todo)_

### git-subtree-push

_(todo)_

### git-subtree-fast

This is a remplacement for `git subtree` which should be _nearly_ functionally equivalent to `git subtree`.
It changes the behavior of `--squash` style subtree forks ***only***. It does not impact other types of subtree
use cases.


## License

Released un GNU GPLv2 in accordance with the license of the original `git-subtree` shell script.
