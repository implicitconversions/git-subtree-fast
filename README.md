# git-subtree-fast

A modified version of `git subtree` optimized for use in `subtree --squash` workflows.

... includes  `subtree-add`, `subtree-pull` and `subtree-push` commands which embed the `--squash`
option and provide a standard process for subtree updating for engineers that more closely
mimics the typicla use case for subtrees or submodules.

## Installation

Use curl/wget to fetch the raw files into a directory of your choice in a given repository.
Typical workflow would be to download the files into either `repo/` or `repo/subtree/` directory.
I like to sandbox all subtrees into a `subtree/` dirto help make it clear to all developers which
directories are in fact subtrees, since it's not immediately clear otherwise which dirs are
subtrees.

A typical installation sequence could look like this:
```
cd /path/to/repo
mkdir subtree && cd subtree
curl -O https://raw.githubusercontent.com/implicitconversions/git-subtree-fast/main/fetch-subtree-tools
./fetch-subtree-tools
```

Updating the subtree tools to latest upstream `main` branch can be done at any time by running the
`fetch-subtree-tools` command.

## Usage

### subtree-add

_(todo)_

### subtree-pull

_(todo)_

### subtree-push

_(todo)_

### git-subtree-fast

This is a remplacement for `git subtree` which should be _nearly_ functionally equivalent to
`git subtree`. It changes the behavior of `--squash` style subtree forks ***only***. It does not
impact other types of subtree use cases.


## License

Released un GNU GPLv2 in accordance with the license of the original `git-subtree` shell script.
