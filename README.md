<br /><br /><br /><div align="center">

![git gud](https://raw.githubusercontent.com/binaryben/dotfiles/docs/public/git%20gud%20dark.png#gh-dark-mode-only)![git gud](https://raw.githubusercontent.com/binaryben/dotfiles/docs/public/git%20gud%20light.png#gh-light-mode-only)

<h1>&nbsp;</h1><br />

![ISC License](https://img.shields.io/badge/license-ISC-green?style=for-the-badge) &nbsp; ![Project Status](https://img.shields.io/badge/status-🚧%20WIP-yellow?style=for-the-badge)

<strong>There are already a LOT of collections of git tools and aliases out there. Here lies another.</strong><br />
<sub>Give your git workflow superpowers with this curated collection of git extensions, related software and aliases. This project aims to make cross provider support easier by bringing the power of `gh`, `tea`, `jira` and `glab` back to a standard interface under `git`. </sub>

<br />

</div>


## New commands

- `git alias` - List available aliases (--help flag will print config.help.aliasname and config.usage.aliasname)
- `git go` - cd to repo or (with --web flag) open repo in browser
- `git draft` - Create a draft PR
- `git pr` - Open PR in browser
- `git ui` - Open repo in terminal UI (shortcut to [GitUI](https://github.com/Extrawurst/gitui), [lazygit](https://github.com/jesseduffield/lazygit) or [tig](https://jonas.github.io/tig/))
- `git ignore` - Generate or modify .gitignore files
- `git sync`
- `git io` - Generate git.io short URLs
- `git orphan` - Create an orphan branch
- `git gud` - Update this repo

### Aliases for [ghq](https://github.com/x-motemen/ghq)

- `git get`
- `git ls`
- `git ll`
- `git root`
- `git create` - will also initialise it and push to remote

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/solar.png)

Goals:

* Cross platform support: Github (Enterprise), Bitbucket and Gitea
* Central git root directory where all projects live and tooling to make working within it easier
* Multiple identity management

### Orphan

```
$ git checkout --orphan gh-pages

# preview files to be deleted
$ git rm -rf --dry-run .
# actually delete the files
$ git rm -rf .
# Create and add new files
```

#### References & Inspiration

- https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases

<details>
<summary>Unholy list of ZSH plugins for git</summary>

TODO: Curate these

* [@peterhurford/git-it-on.zsh](https://github.com/peterhurford/git-it-on.zsh)
* [@unixorn/bitbucket-git-helpers.plugin.zsh](https://github.com/unixorn/bitbucket-git-helpers.plugin.zsh)
* [@unixorn/git-extra-commands](https://github.com/unixorn/git-extra-commands)
* [@zimfw/git](https://github.com/zimfw/git)
* [@sebastiangraz/c](https://github.com/sebastiangraz/c)
* [@bossjones/boss-git-zsh-plugin](https://github.com/bossjones/boss-git-zsh-plugin)
* [@gimbo/gimbo-git.zsh](https://github.com/gimbo/gimbo-git.zsh)
* [@robertzk/send.zsh](https://github.com/robertzk/send.zsh)
* [@MenkeTechnologies/zsh-git-acp](https://github.com/MenkeTechnologies/zsh-git-acp)
* [@aswitalski/oh-my-zsh-sensei-git-plugin](https://github.com/aswitalski/oh-my-zsh-sensei-git-plugin)
* [@caarlos0-graveyard/git-add-remote](https://github.com/caarlos0-graveyard/git-add-remote)
* [@aswitalski/oh-my-zsh-opera-git-plugin](https://github.com/aswitalski/oh-my-zsh-opera-git-plugin)
* [@mdumitru/git-aliases](https://github.com/mdumitru/git-aliases)
* [@peterhurford/git-aliases.zsh](https://github.com/peterhurford/git-aliases.zsh)
* [@Schroefdop/git-branches](https://github.com/Schroefdop/git-branches)
* [@LucasLarson/gunstage](https://github.com/LucasLarson/gunstage)
* [@gobriansteele/git-clean-branch](https://github.com/gobriansteele/git-clean-branch)
* [@rapgenic/zsh-git-complete-urls](https://github.com/rapgenic/zsh-git-complete-urls)
* [@caarlos0-graveyard/zsh-open-pr](https://github.com/caarlos0-graveyard/zsh-open-pr)
* [@lyze/posh-git-sh](https://github.com/lyze/posh-git-sh)
* [@unixorn/git-extra-commands](https://github.com/unixorn/git-extra-commands)
* [@bigH/git-fuzzy](https://github.com/bigH/git-fuzzy)
* [@laggardkernel/git-ignore](https://github.com/laggardkernel/git-ignore)
* [@aubreypwd/zsh-plugin-git-is-clean](https://github.com/aubreypwd/zsh-plugin-git-is-clean)
* [@capsulescodes/more-hooks-for-git](https://github.com/capsulescodes/more-hooks-for-git)
* [@peterhurford/git-it-on.zsh](https://github.com/peterhurford/git-it-on.zsh)
* [@nekofar/zsh-git-lfs](https://github.com/nekofar/zsh-git-lfs)
* [@rcruzper/zsh-git-plugin](https://github.com/rcruzper/zsh-git-plugin)
* [@mroth/git-prompt-useremail](https://github.com/mroth/git-prompt-useremail)
* [@ytakahashi/igit](https://github.com/ytakahashi/igit)
* [@diazod/git-prune](https://github.com/diazod/git-prune)
* [@git-time-metric/gtm-terminal-plugin](https://github.com/git-time-metric/gtm-terminal-plugin)
* [@packruler/zsh-git-scripts](https://github.com/packruler/zsh-git-scripts)
* [@sobolevn/git-secret](https://github.com/sobolevn/git-secret)
* [@seletskiy/zsh-git-smart-commands](https://github.com/seletskiy/zsh-git-smart-commands)
* [@jelek21/omz-git-smart-commands](https://github.com/jelek21/omz-git-smart-commands)
* [@caarlos0-graveyard/zsh-git-sync](https://github.com/caarlos0-graveyard/zsh-git-sync)
* [@dehlen/git-tree-zsh](https://github.com/dehlen/git-tree-zsh)
* [@alexiszamanidis/zsh-git-fzf](https://github.com/alexiszamanidis/zsh-git-fzf)
* [@egyptianbman/zsh-git-worktrees](https://github.com/egyptianbman/zsh-git-worktrees)
* [@davidde/git](https://github.com/davidde/git)
* [@SukkaW/zsh-gitcd](https://github.com/SukkaW/zsh-gitcd)
* [@viko16/gitcd.plugin.zsh](https://github.com/viko16/gitcd.plugin.zsh)
* [@tevren/gitfast-zsh-plugin](https://github.com/tevren/gitfast-zsh-plugin)
* [@grimmbraten/gitgo](https://github.com/grimmbraten/gitgo)
* [@ltj/gitgo](https://github.com/ltj/gitgo)
* [@buzuloiu/zsh-github-folders](https://github.com/buzuloiu/zsh-github-folders)
* [@shakir-abdo/zsh-github-plugin](https://github.com/shakir-abdo/zsh-github-plugin)
* [@voronkovich/gitignore.plugin.zsh](https://github.com/voronkovich/gitignore.plugin.zsh)
* [@denysdovhan/gitio-zsh](https://github.com/denysdovhan/gitio-zsh)
* [@nicolodiamante/gitio](https://github.com/nicolodiamante/gitio)
* [@xylous/gitstatus](https://github.com/xylous/gitstatus)
* [@washtubs/gitsync](https://github.com/washtubs/gitsync)
* [@wfxr/forgit](https://github.com/wfxr/forgit)
* [@MisterRios/stashy](https://github.com/MisterRios/stashy)
* [@robin-mbg/switch-git](https://github.com/robin-mbg/switch-git)

</details>