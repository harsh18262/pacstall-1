<p align="center">
<a href="https://github.com/pacstall/pacstall/releases/latest"><img src="https://img.shields.io/github/v/release/pacstall/pacstall?color=red&style=flat-square"></a>
<a href="https://www.gnu.org/software/bash/"><img src="https://img.shields.io/badge/bash-v5-brightgreen?style=flat-square&logo" alt="Bash v5"></a>
  <a href="https://github.com/pacstall/pacstall/issues"><img src="https://img.shields.io/github/issues/pacstall/pacstall?style=flat-square"></a>
<a href="https://github.com/pacstall/pacstall/actions?query=workflow%3A%22test+install+script%22"><img src="https://img.shields.io/github/workflow/status/pacstall/pacstall/test%20install%20script?style=flat-square"></a>
<a href="https://www.codefactor.io/repository/github/pacstall/pacstall"><img src="https://img.shields.io/codefactor/grade/github/pacstall/pacstall/develop?style=flat-square"></a>
<a href="https://discord.gg/yzrjXJV6K8"><img src="https://img.shields.io/discord/839818021207801878?style=flat-square"></a>
<a href="https://matrix.to/#/#pacstall:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
<a href="https://www.reddit.com/r/pacstall/"><img src="https://img.shields.io/reddit/subreddit-subscribers/pacstall?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAACXBIWXMAATRQAAE0UAFXCOjxAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAaBJREFUKJF9kk9LVGEUxn/nzlXT8TqaSPoBRPAjBANC3lUKglQatLY2zU78Bu4NImp2OYi4HLCFilpg+0Lxz06woAgdveaMNvO0eOfODI30wAsv7znPc855z2M0QCP008JLYBwYrD4fAXmKvLJPfI9zrUZ6wBTGW4yA2yAuMGZsjSUAr0byyDWRUn3gJaDnHnSmAmBRozwFMI3Qj8/hrZUmMlD4AU/mYG8HFl64yiWG/OpMzSQzR9pcgi/bULqKhwtoJeNXP6KO9gDSkzB8H4K7cCcJH1fg8rxBlHEUUlSI9DojXUXS2U814fyXi2XnpBBplGuvppLwnfrJEUz2QnQKlwV41AfH+y7m1dNRyFeFSGMdUrksRQXpQ1aqlN1ZfSddnEqVijSRiivuekAegNJvWH8PyS7o6oXdHdj77O6d3bC17DpwO82b0gzQxgFGQMKHx7PwcAaui4CgrQNWs7A8D39uQEQYQ1ZtdxpYjA0BQLLb+So6a3SPEM9sg1zdcs4Rb/5juQjx3DbIuY00xtIM0EoG+8fkIo/Hgq3xLc79CzNQvfQ4D27CAAAAAElFTkSuQmCC"></a>
<a href="https://github.com/pacstall/pacstall-programs"><img src="https://img.shields.io/github/commit-activity/m/pacstall/pacstall-programs?style=flat-square&label=user%20repo%20activity"></a>
</p>

<p align="center"><b>PACSTALL</b></p>
<p align="center">
<a href="https://github.com/pacstall/pacstall"><img align="center" src="https://pacstall.dev/image/pacstall.svg" alt="Pacstall Logo"></a>
</p>
<p align="center"><b>The AUR Ubuntu never had</b></p>

<p align="center">Pacstall will attempt to become the AUR Ubuntu wishes it had. It takes the AUR and puts a spin on it, making it easier to install programs without scouring github repos and the likes.</p>
<p align="center">The list of available packages can be found <a href="https://github.com/pacstall/pacstall-programs/tree/master/packages">here</a>.</p>
</p>

---

### Features

*  Supports binary, git, appimage, building and `.deb` packages
*  Accelerated package download using [axel](https://github.com/axel-download-accelerator/axel)*
*  Auto update checks for git packages, so you always get the latest build of your favourite program off the latest commit by the developer
*  Over 175 packages available to install in the official programs repository
*  Ability to install programs from multiple repositories
*  Ability to track Pacstall updates from any fork/branch easily
*  Completions available for `bash` (`ZSH`), and `fish`

*\* marked features are optional, and can be turned on during installation*

---

### Installing

You can run the command below to install Pacstall.
You can also grab the deb file [here](https://github.com/pacstall/pacstall/releases/latest) but it may be a bit older.
```bash
sudo bash -c "$(curl -fsSL https://git.io/JsADh || wget -q https://git.io/JsADh -O -)"
```

### Uninstalling

You can run the command below to uninstall Pacstall.
```bash
bash -c "$(curl -fsSL https://git.io/JEZbi || wget -q https://git.io/JEZbi -O -)"
```
---

### Basic Commands
```bash
pacstall -I foo
``` 
This will install foo. Equivalent of apt install

```bash
pacstall -R foo
```
This will remove foo. Equivalent of apt remove

```bash
pacstall -S foo
```
This will search for foo in repositories. Equivalent of apt search

```bash
pacstall -A
```
Run this command with a github/gitlab url to add a repo

```bash
pacstall -U
```
This will update pacstall's scripts

```bash
pacstall -Up
```

This will update packages. Equivalent of apt upgrade

These are the basic commands, for more info, run `pacstall -h`

---
### Auto completions
Pacstall has fully supported auto completions for the `bash`, and `fish` shells. For the `ZSH` shell you can emulate the completions using the following commands.
#### Zsh auto completion
Zsh can emulate bash completion scripts by default so all you have to do is add these to your `.zshrc` or wherever you source things:
```bash
autoload bashcompinit
bashcompinit
source /usr/share/bash-completion/completions/pacstall
```

### License
---
![GPLv3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)
```monospace
Pacstall is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, version 3 of the License

Pacstall is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Pacstall. If not, see <https://www.gnu.org/licenses/>.
```
