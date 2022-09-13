<blockquote><details><summary>⚠️ <strong>State of Development</strong> - click to read</summary><br />

👋 G'day! Thanks for checking out my project. This project is in a very early stage of development. There is much to do. Please be aware, here be dragons!

</details></blockquote>

<br /><br /><br /><div align="center">

![git gud](https://raw.githubusercontent.com/binaryben/dotfiles/docs/public/git%20gud%20dark.png#gh-dark-mode-only)![git gud](https://raw.githubusercontent.com/binaryben/dotfiles/docs/public/git%20gud%20light.png#gh-light-mode-only)

<h1>&nbsp;</h1><br />

![ISC License](https://img.shields.io/badge/license-ISC-green?style=for-the-badge) &nbsp; ![Project Status](https://img.shields.io/badge/status-🚧%20WIP-orange?style=for-the-badge)

<strong>There are already a LOT of collections of git tools and aliases out there. Here lies another.</strong><br />
<sub>Give your git workflow superpowers with this meticulously curated collection of extra git commands, related software and some cool aliases and functions for good measure. This project has several ambitious goals. One of the most noteworthy is to make cross provider support easier by bringing the power of `gh`, `tea`, `jira`, `glab` and others back into a standard interface under `git` itself.</sub>

<br />

![Placeholder for an animated demo](https://raw.githubusercontent.com/zalog/placeholder-loading/master/docs/imgs/placeholder-loading-demo-3.gif)

</div>

## 🎯 &nbsp; Goals

* Cross platform support:
  * Git repository hosting platforms: Github (inc. Enterprise), Bitbucket, Gitea and Gitlab
  * Operating systems: Linux, macOS and Windows (via Git Bash)
* Prioritise use of a central git root directory where all projects live with tooling to make working within it easier (akin to `go get`)
* Manage multiple git identities - keep work and personal life separate
* Add convenience functions, utilities and mnemonics
* Install common extensions automatically

## 🙅 &nbsp; Non-goals

* Short aliases like `alias g=git` and `alias gc=git commit`
  * Everyone tends to have very individual preferrences, so you're better off managing them in your own dotfiles
  * Some functions that could be used as global aliases have been created, but won't be aliased by default - i.e. check out the `gud-gg` script for which a lazy programmer might add `alias gg=gud-gg` to their dotfiles
* Anything that is going to really mess up common workflows
* Mandating ways of working within git repos (i.e. this won't force git flow on you)

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

<details>
<summary> &nbsp; <small><em>Click heading to show / hide</em></sup><br /><h2>📖 &nbsp; Table of contents</h2></summary><br />

<br />

* 🎯 &nbsp; [**Goals & Non-goals**](#--goals)
* 📖 &nbsp; [**Table of contents**](#--table-of-contents)
* ⌛️ &nbsp; [**Quick start**](#%EF%B8%8F--quick-start)
* 🧠 &nbsp; [**Philosophy**](#--philosophy)
* 😱 &nbsp; [**Extended commands**](#--extended-commands)
* 🧭 &nbsp; [**Repo management**](#--repo-management)
  * ➤ [Repos](#--repos)
  * ➤ [Users](#--users)
  * ➤ [Remote](#--remote)
  * ➤ [Workflow](#--workflow)
* [**New commands**](#)
  * ➤ [Utilities](#)
  * ➤ [New verbs](#)
  * ➤ [New namespaces](#)

<br />

</details>

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## ⌛️ &nbsp; Quick start

🤷‍♂️ Probably ZSH plugin is the fastest way for those who wanna try it. I guess I will need to implement that.

Otherwise...

1. Clone project
2. Add `./bin` to path
3. Include `./git-gud-aliases` in `~/.gitconfig`
4. `git gud install`

... will be the likely workflow

🍺 Homebrew support is a probably a good idea as well

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## 🧠 &nbsp; Philosophy

Git is a very powerful but complex piece of software. It is natural to want to make something complex easier to use. 

I am slightly wary that Microsoft is setting up to roll out their E3 business strategy again with the `gh` tool. This is an effort to comodotise Github again and fight back against it becoming a massive walled garden.

<!-- https://github.com/freemountain/tea/blob/master/FEATURE-COMPARISON.md#philosophy -->

To reduce cognitive overload, the following decision framework was made:

* Extend builtin commands where practical
* Limit the number of new subcommands

This allows better scripting options and makes it easier to work in the terminal without having to worry about where the project is actually hosted (you know, because decentralised and standardied was the goal of using `git` in the first place).

The developer only needs to remember a handful of extra things to get the most from this package:

1. You can check if any built command has any superpowers by running it with `--superpowers`
2. Remote git repo hosting platforms are managed in `git` now, and done in a fairly intuitive manner. Things like `git pr` work as expected for example.
3. 

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## 😱 &nbsp; Extended commands

*Git Gud* uses the [git-extend](https://github.com/nickolasburr/git-extend) project to extend the built in commands of `git`. This may cause some potential users of *Git Gud* to scream in disgust and run away. I encourage you to try it out though ... then you can run. Every effort has been made to keep it as seemless as possible without causing any [breaking changes to existing workflows](https://xkcd.com/1172/).

> ℹ️ Once *Git Gud* is installed, explore what changes have been made by appending `--goodies`, `--superpowers`, `--extras` or `--helpers` to any built in command. (it must be the first parameter to work, i.e. `git show --goodies`). If git complains about invalid arguments/usage, the command has not been extended. Otherwise helpful information will be displayed.

<!--

List of other common commands that could be overstuffed (and reasons why it was decided not to, if any)

git bisect
git clean
git clone - will just use `git get` instead which will hopefully be aliased to `gg` by many
git commit
git config
git diff
git fetch
git grep
git init
    - I really want to overstuff this with some interactive project creation wizards or similar
    - Am sick of making repos in the browser first
    - Create README, gitignore, create on origin and push to origin
git mv
git rebase
git remote
git reset
git restore
git revert
git switch

-->

<details><summary><strong>Click to show the list of <del>butchered</del> supercharged commands ...</strong></summary><br />

<details><summary><code>git add</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

</details>
<details><summary><code>git branch</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

</details>
<details><summary><code>git checkout</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

Incorporate from `git-extra-commands`:

* `git-checkout-branches`
* `git-checkout-by-date`
* `git-checkout-default-branch`

</details>
<details><summary><code>git diff</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

</details>
<details><summary><code>git log</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

</details>
<details><summary><code>git merge</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

Incorporate from `git-extra-commands`:

* git-improved-merge

</details>
<details><summary><code>git pull</code></summary><br />

🚧 Coming soon

Incorporate from `git-extra-commands`:

* `git-superpull`

</details>
<details><summary><code>git push</code></summary><br />

🚧 Coming soon

Incorporate from `git-extra-commands`:

* `git-sp` - add as a flag to built in `push` (maybe also add `git sp` as an alias?)

</details>
<details><summary><code>git reflog</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

</details>
<details><summary><code>git rm</code></summary><br />

🚧 Coming soon

Incorporate from `git-extra-commands`:

* `git-submodule-rm`
* `--clean` - `git-rm-deleted-from-repo`
* `--dangling-commits` - git-delete-dangling-commits
* `--local-merged` - git-delete-local-merged
* `--merged-branches` - git-delete-merged-branches
* `--remote-branch` - git-delete-remote-branch
* `--squashed-and-merged-branches` - git-delete-squashed-and-merged-branches
* `--tag` - git-delete-tag

Add a `--nuke` flag that totally destroys the object both locally and remotely:

> 🚨 Very destructive!

* `--nuke`
  - `repo`
  - `branch` - `git-nuke`
  - `file` - `git-purge-from-history`
  - `local` - `git-reset-with-fire`

</details>
<details><summary><code>git show</code></summary><br />

🚧 Coming soon

Useful functions to provide insights into the repo you are working in

Incorporate from `git-extra-commands`:

* `git show` - show various useful data
  - `--big-files`
  - `--branches-that-touch`
  - `--changes` - git-what-the-hell-just-happened
  - `--children-of-commit`
  - `--churned-files` - git-churn
  - `--commit-in-release` - git-where
  - `--common-ancestors` - git-oldest-common-ancestor
  - `--conflicts` - git-conflicts
  - `--default-branch` - git-remote-default-branch
  - `--divergence`
  - `--ignored` - Files in the repo being ignored because of `.gitignore`
  - `--incoming` - git-incoming
  - `--last-diff`
  - `--neck` - git-neck (counterpart to `--neck`)
  - `--outgoing` - git-outgoing
  - `--recent-changes` - git-recent
  - `--recently-checkedout-branches` - git-recently-checkedout-branches
  - `--related` - git-related
  - `--relationship` - git-rel
  - `--trail` - git-trail (counterpart to `--neck`)
  - `--unreleased` - git-unreleased
  - `--unpushed` - git-unpushed
  - `--when-merged` - git-when-merged

</details>
<details><summary><code>git stash</code></summary><br />

🚧 Coming soon

Make it behave a bit nicer - see [@MisterRios/stashy](https://github.com/MisterRios/stashy)

</details>
<details><summary><code>git status</code></summary><br />

🚧 Coming soon

Will have whatever the boilerplate provided by `git-extend` supplies to start with.

</details>
<details><summary><code>git tag</code></summary><br />

🚧 Coming soon

Incorporate from `git-extra-commands`:

* `git-tag-diff` as `--diff`
* `git-tag-and-sign` - can we autosign based on profile?

</details>
<details><summary><code>git undo</code></summary><br />

🚧 Coming soon

Incorporate from `git-extra-commands`:

* `git-undo`
* `git-undo-push`
* `git-undelete`

</details>

</details>

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

<!-- 

Sorting 'git-extra-commands' into nicer name spaces

git-add-username-remote
git-age
git-amend-all
git-branch-rebaser
git-branches-that-touch
git-change-log
git-clone-subset
git-comma
git-cut-branch
git-edit-conflicts
git-files
git-find-dirty
git-flush
git-force-mtimes
git-forest
git-functionlog
git-history-graph
git-lines
git-ls-branch-files
git-ls-object-refs
git-maxpack
git-move-commits
git-object-deflate
git-overwritten
git-pie-ify
git-plotrepo
git-promote
git-prune-branches
git-pruneall
git-pylint
git-rebase-authors
git-rebase-theirs
git-ref-recent
git-remove-conflicts ours or theirs FILES...
git-rename-branches
git-restore-mtime
git-reup
git-run-command-on-revisions
git-shamend
git-show-overwritten
git-shrink-repo
git-side-by-side
git-stats
git-track
git-up

-->

## 🧭 &nbsp; Repo management

**AKA: Universal git repository hosting platform management**

These commands are designed to provide a standard interface to a number of platform specific tools. Running `git gud install` will ensure the needed dependencies are also installed to make this work seamlessly. This includes: `gh`, [tea](https://github.com/freemountain/tea/tree/master), [jira](https://github.com/ankitpokhrel/jira-cli), [glab](https://glab-cli.io/)

### ➤ &nbsp; Repos

These commands help the developer get existing repositories from the supported platforms, and helps them navigate faster.

<details><summary><code>git get</code></summary><br />

* `git get` - [ghq](https://github.com/x-motemen/ghq) alias (with some conveniences added)

</details>
<details><summary><code>git go</code></summary><br />

* `git go` - cd to repo directory

</details>
<details><summary><code>git open</code></summary><br />

<!-- git-github-open -->

* `git open` - open repo/file/pr/commit/issue in browser (alias as `git browse` as well)

</details>

#### Other related functions

* `gud gg` - smarter combination of `git get`, `git go` and `git open`; useful to alias to `gg`

#### Supported platforms

| Command | Github | Bitbucket | Gitea | GitLab |
| ------- | ------ | --------- | ----- | ------ |
| get     |   ﹖   |     ﹖     |  ﹖   |   ﹖   |
| open    |   ﹖   |     ﹖     |  ﹖   |   ﹖   |

### ➤ &nbsp; Users

Manage which credentials and identities work wiith which providers using these tools

<details><summary><code>git profile</code></summary><br />

* `git profile` - Create or manage user profiles
  - `auth`
  - `config`
  - `email`
  - `gpg`
  - `name`
  - `select`
  - `ssh`

</details>
<details><summary><code>git whoami</code></summary><br />

* `git whoami` - show `user.name <user.email>` based on the repo you are. Also show profile information

</details>

#### Supported platforms

| Command | Github | Bitbucket | Gitea | GitLab |
| ------- | ------ | --------- | ----- | ------ |
| profile |   ﹖   |     ﹖     |  ﹖   |   ﹖   |

### ➤ &nbsp; Remote

All the things that make git a truly collaborative experience are here

<details><summary><code>git issue</code></summary><br />

* `git issue` - Create or manage issues

</details>
<details><summary><code>git pr</code></summary><br />

<!--

git-github-open
git-gitlab-mr
git-checkout-pr
git-where-pr
git-pr-fetch
git-pr-list
git-fetch-prs

-->

* `git pr` - Manage PR in CLI or open PR in browser
    - Create a draft PR

</details>
<details><summary><code>git publish</code></summary><br />

* `git publish` - see `git-publish` for inspiration

</details>
<details><summary><code>git release</code></summary><br />

<!-- git-release-tag - create a github release for a specified tag -->

* `git release` - 

</details>
<details><summary><code>git topic</code></summary><br />

* `git topic` - Change the topic on the repo page

</details>

#### Supported platforms

| Command | Github | Bitbucket | Gitea | GitLab |
| ------- | ------ | --------- | ----- | ------ |
| issue   |   ﹖   |     ﹖     |  ﹖   |   ﹖   |
| pr      |   ﹖   |     ﹖     |  ﹖   |   ﹖   |
| publish |   ﹖   |     ﹖     |  ﹖   |   ﹖   |
| release |   ﹖   |     ﹖     |  ﹖   |   ﹖   |
| topic   |   ﹖   |     ﹖     |  ﹖   |   ﹖   |

### ➤ &nbsp; Workflow

Tools that come under the development workflows

<details><summary><code>git dev</code></summary><br />

* `git dev` - Startup dev workflows (local and remote)

</details>
<details><summary><code>git gist</code></summary><br />

* `git gist` - 

</details>
<details><summary><code>git tasks</code></summary><br />

* `git tasks` - Github Actions (`gh workflow` / `gh run`), CI, etc

</details>

#### Supported platforms

| Command |   Github   | Bitbucket | Gitea | GitLab |
| ------- | ---------- | --------- | ----- | ------ |
| dev     | Codespaces |     ﹖     |  ﹖   |   ﹖   |
| gist    |     ✅     |     ﹖     |  ﹖   |   ﹖   |
| tasks   |   Actions  |     ﹖    |  ﹖   |   ﹖   |

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## 🧑‍💻 &nbsp; New commands

Git Gud adds a number of extra subcommands to your local `git` installation. 

<!--

These leading letters have no commands, or arguably none that will get used in common usage. This makes them important in terms of making aliasable commands.

For example, n is ideal for git new / gn, which could be used as a smart function for making a new repo or branch.

e (env--helper), j, k, n (name-rev & notes), o, q (quiltimport), ~u (unpack-*, update-*, unload-*), ~v (var, verify-*, version), x, y, z

Working ideas for aliases:

e: 
j: 
k: 
n: 
o: 
q: 
u:
  `gu` → `git utils`
  `gui` → `git ui` → 
v: 
x: 
y: 
z: `gz` → `get go` → fzf path in repo (akin to zoxide/z)

-->

### ➤ &nbsp; Namespaced

<details><summary><code>git author</code></summary><br />

Very useful for blaming or thanking authors, as well as for trying to figure out who can help with a problem.

Some of these might be flags. Will need to plan how to make it all work as a unified command that matches the rest of the git DX.

* `git author`
  - `change` - `git-change-author`, `git-replace-author`
  - `credit` - `git-credit`
  - `contributions` - `git-rank-contributors`
  - `current` - List current authors in the repository in descending commit-count order. `git-authors`
  - `historic`
  - `mvp` - Top 10 authors by number of commits and by number of lines changed `git-winner`
  - `wordy` - Sort authors by commit message length `git-wordiness`

</details>
<details><summary><code>git ui</code></summary><br />

Run different commands using a terminal-based GUI (TUI) instead of the command line.

Supported packages:

* [GitUI](https://github.com/Extrawurst/gitui)
* [lazygit](https://github.com/jesseduffield/lazygit)
* [tig](https://jonas.github.io/tig/)

Supported actions:

* `git ui` - Open repo in terminal UI
  * `add`
  * `commit`
  * ?

</details>
<details><summary><code>git utils</code></summary><br />

A collection of useful functions that are used with git.

> It's recommended to alias `gu` to `git utils` since there is limited subcommands in git starting with 'u'.

* `git utils`
  - `git ignore` - `git-make-gitignore`
  - `git io` - Generate git.io short URLs (proposed: add support for custom url shortners)
  - `git replay` - scrub through git commits, forwards and backwards (see `git-jump`)
  - `git summary` - prettier `git status` (see `git wtf`)

</details>

### ➤ &nbsp; Verbs

<details><summary><code>git ls</code></summary><br />

List various objects in a number of ways.

* `git ls` (suggested aliases `ls` and `ll`)
  - `branch` - `git-branch-status`, git-current-branch
    - `--upstream` - git-upstream-name
  - `commit` - git-current-commit
    - `--merged` - `git-merged-branches`
  - `diff` - partially inspired by the idea of `git-maildiff`, but for piping into `clip` or similar
  - `files` - builtin `git ls-files`
    - `--deleted` - `git-attic`
  - `remote` - builtin `git ls-remote`
  - `repo`
    - `--default-branch` git-origin-head
  - `root` - echo global project root(s) (via ghq) or root of current repo (git-root-directory, with --local flag)
  - `tags` - `git-tags`, `git-taglist`
  - `tree` - builtin `git ls-tree`
  - `stats` - print summary of changes (for prompt/status bars)
    - `--oneline` - put them all on one line

Options:

* `--longlist -l` - show extra information
* `--pretty` - print in colour and with Nerd Font icons (useful for $PROMPT/$PS1 in conjunction with `--limit=1`)
* `--limit=n` - just get n item(s)
* `--format=json` - option to get data in json to pipe into `jq`

</details>
<details><summary><code>git new</code></summary><br />

* `git new` (also alias `create`)
  - `repo` will also initialise it and push to remote
  - `branch`
  - `orphan`

<!--

How to orphan:

$ git checkout --orphan gh-pages

# preview files to be deleted
$ git rm -rf --dry-run .
# actually delete the files
$ git rm -rf .
# Create and add new files

-->

</details>
<details><summary><code>git search</code></summary><br />

* `git search` - Fuzzy find things (using `fzf`)
  - `commit` - git-commit-browser
  - `checkout` - git-checkout-commit, git-checkout-preview
  - `add` - git-fzf-add
  - `log` - git-fzf-log-browser, git-fzf-pickaxe-browser
  - `reflog` - git-fzf-reflog-browser
  - `switch` - git-sr

</details>

### ➤ &nbsp; Functions

These subcommands are convenience functions. They are wrappers around other commands, usually with the intention of turning multi-step workflows into one command. 

New subcommands like these should be added very sparingly to avoid polluting the global namespace and to avoid adding to the developers cognitive workload. In some cases though, it makes sense to bring some functionality to the top level of `git`, escpecially for workflows that are performed several times a day.

* `git alias` - List available aliases (--help flag will print config.help.aliasname and config.usage.aliasname)
* `git co` - `git checkout` if a branch is named (also incorporate `git-switch-branch`), else start a fzf branch chooser
* `git git` - Fix common typo (especially when copy and pasting commands)
* `git unstage` - [@LucasLarson/gunstage](https://github.com/LucasLarson/gunstage)
* `git sync` - combination of `git-upstream-sync`, [@caarlos0-graveyard/zsh-git-sync](https://github.com/caarlos0-graveyard/zsh-git-sync) and [@washtubs/gitsync](https://github.com/washtubs/gitsync)

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## 🔋 &nbsp; Included extensions

* `git gud`
  - `update`
  - `install`
  - `completion`
* `git lfs` - [Large File Storage](https://git-lfs.github.com/)
* `git secret` - [@sobolevn/git-secret](https://github.com/sobolevn/git-secret)
* `git time` - Time tracking integration

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

#### References & Inspiration

- https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases

<details>
<summary>Unholy list of ZSH plugins for git</summary>

TODO: Curate these

* [@alexiszamanidis/zsh-git-fzf](https://github.com/alexiszamanidis/zsh-git-fzf)
* [@aswitalski/oh-my-zsh-opera-git-plugin](https://github.com/aswitalski/oh-my-zsh-opera-git-plugin)
* [@aubreypwd/zsh-plugin-git-is-clean](https://github.com/aubreypwd/zsh-plugin-git-is-clean)
* [@bigH/git-fuzzy](https://github.com/bigH/git-fuzzy)
* [@buzuloiu/zsh-github-folders](https://github.com/buzuloiu/zsh-github-folders)
* [@caarlos0-graveyard/git-add-remote](https://github.com/caarlos0-graveyard/git-add-remote)
* [@caarlos0-graveyard/zsh-git-sync](https://github.com/caarlos0-graveyard/zsh-git-sync)
* [@caarlos0-graveyard/zsh-open-pr](https://github.com/caarlos0-graveyard/zsh-open-pr)
* [@capsulescodes/more-hooks-for-git](https://github.com/capsulescodes/more-hooks-for-git)
* [@dehlen/git-tree-zsh](https://github.com/dehlen/git-tree-zsh)
* [@denysdovhan/gitio-zsh](https://github.com/denysdovhan/gitio-zsh)
* [@diazod/git-prune](https://github.com/diazod/git-prune)
* [@egyptianbman/zsh-git-worktrees](https://github.com/egyptianbman/zsh-git-worktrees)
* [@git-time-metric/gtm-terminal-plugin](https://github.com/git-time-metric/gtm-terminal-plugin)
* [@gobriansteele/git-clean-branch](https://github.com/gobriansteele/git-clean-branch)
* [@grimmbraten/gitgo](https://github.com/grimmbraten/gitgo)
* [@jelek21/omz-git-smart-commands](https://github.com/jelek21/omz-git-smart-commands)
* [@laggardkernel/git-ignore](https://github.com/laggardkernel/git-ignore)
* [@ltj/gitgo](https://github.com/ltj/gitgo)
* [@lyze/posh-git-sh](https://github.com/lyze/posh-git-sh)
* [@mroth/git-prompt-useremail](https://github.com/mroth/git-prompt-useremail)
* [@nicolodiamante/gitio](https://github.com/nicolodiamante/gitio)
* [@packruler/zsh-git-scripts](https://github.com/packruler/zsh-git-scripts)
* [@peterhurford/git-aliases.zsh](https://github.com/peterhurford/git-aliases.zsh)
* [@peterhurford/git-it-on.zsh](https://github.com/peterhurford/git-it-on.zsh)
* [@rapgenic/zsh-git-complete-urls](https://github.com/rapgenic/zsh-git-complete-urls)
* [@rcruzper/zsh-git-plugin](https://github.com/rcruzper/zsh-git-plugin)
* [@robertzk/send.zsh](https://github.com/robertzk/send.zsh)
* [@robin-mbg/switch-git](https://github.com/robin-mbg/switch-git)
* [@Schroefdop/git-branches](https://github.com/Schroefdop/git-branches)
* [@seletskiy/zsh-git-smart-commands](https://github.com/seletskiy/zsh-git-smart-commands)
* [@shakir-abdo/zsh-github-plugin](https://github.com/shakir-abdo/zsh-github-plugin)
* [@SukkaW/zsh-gitcd](https://github.com/SukkaW/zsh-gitcd)
* [@tevren/gitfast-zsh-plugin](https://github.com/tevren/gitfast-zsh-plugin)
* [@unixorn/bitbucket-git-helpers.plugin.zsh](https://github.com/unixorn/bitbucket-git-helpers.plugin.zsh)
* [@viko16/gitcd.plugin.zsh](https://github.com/viko16/gitcd.plugin.zsh)
* [@voronkovich/gitignore.plugin.zsh](https://github.com/voronkovich/gitignore.plugin.zsh)
* [@wfxr/forgit](https://github.com/wfxr/forgit)
* [@xylous/gitstatus](https://github.com/xylous/gitstatus)
* [@ytakahashi/igit](https://github.com/ytakahashi/igit)

</details>

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## 🎗 &nbsp; Contributing

I might sell Git Gud stickers and shirts actually. Could be fun...

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

## 🙏 Thanks!

As with any open source project, this one is also built on the good work of others.

### ➤ &nbsp; *Git Gud* logo

The Git Gud logo is remixed from the Git [Logo](https://git-scm.com/downloads/logos) by [Jason Long](https://twitter.com/jasonlong) under the [Creative Commons Attribution 3.0 Unported License](https://creativecommons.org/licenses/by/3.0/). Thanks for giving your awesome design to the open-source community so freely Jason!

> **Disclaimer:** This project is in no way affiliated with or sponsored by the git project, or its' maintainers. This is not in any way an "official" git project.

### ➤ &nbsp; Joe Blocks

Big thanks to **Joe Blocks** ([@unixorn](https://github.com/unixorn)) and his [extra-git-commands](https://github.com/unixorn/git-extra-commands) project. Most of the foundational work for this project is based of his collection and work.

### ➤ &nbsp; Inspiration for short aliases

Thanks to the authors of these repositories which I referenced whilst creating my own [short aliases for git](https://github.com/binaryben/dotfiles/blob/main/config/git/git.aliases.sh). These repositories are primarily simple aliases, but there are a few neat functions as well. Hopefully they may inspire you too.

* [Oh My Zsh!](https://github.com/ohmyzsh/ohmyzsh/blob/c99f3c50fa46a93be28be88632889404fff3b958/plugins/git/README.md#aliases)
* [@aswitalski/oh-my-zsh-sensei-git-plugin](https://github.com/aswitalski/oh-my-zsh-sensei-git-plugin)
* [@bossjones/boss-git-zsh-plugin](https://github.com/bossjones/boss-git-zsh-plugin)
* [@gimbo/gimbo-git.zsh](https://github.com/gimbo/gimbo-git.zsh)
* [@mdumitru/git-aliases](https://github.com/mdumitru/git-aliases)
* [@MenkeTechnologies/zsh-git-acp](https://github.com/MenkeTechnologies/zsh-git-acp)
* [@sebastiangraz/c](https://github.com/sebastiangraz/c)
* [@zimfw/git](https://github.com/zimfw/git)
* [@nekofar/zsh-git-lfs](https://github.com/nekofar/zsh-git-lfs)
* [@davidde/git](https://github.com/davidde/git)
