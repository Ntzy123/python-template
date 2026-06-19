<h1 style="text-align:center" align="center">这是一个模板</h1>

# Linux 常用软件清单

## 包管理器可直接安装

btop、curl、wget、unzip、git、nvim、nano、make、python3、pip、venv、lsd、fd、zoxide、yazi、dust、bat、fzf、less、openssh-server、openssh-client、rg、zsh、lazygit

## 需 GitHub 仓库

| 组件                         | GitHub 仓库                                                  |
| ---------------------------- | ------------------------------------------------------------ |
| Oh My Zsh                    | https://github.com/ohmyzsh/ohmyzsh                           |
| zsh-autosuggestions          | https://github.com/zsh-users/zsh-autosuggestions             |
| zsh-syntax-highlighting      | https://github.com/zsh-users/zsh-syntax-highlighting         |
| Starship                     | https://github.com/starship/starship                         |
| LazyVim                      | https://github.com/LazyVim/LazyVim                           |
| CaskaydiaCove Nerd Font Mono | https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/CascadiaCode.zip |

------

## 安装命令

### Arch Linux

```bash
sudo pacman -S --needed btop curl wget unzip git neovim nano make python python-pip python-venv \
  lsd fd zoxide yazi dust bat fzf less openssh ripgrep zsh lazygit
```

### Fedora

```bash
sudo dnf install -y btop curl wget unzip git neovim nano make python3 python3-pip python3-virtualenv \
  lsd fd-find zoxide yazi dust bat fzf less openssh-server openssh-clients ripgrep zsh lazygit
```

>   ⚠️ `fd`包名为 `fd-find`，命令仍为 `fd`。

### Ubuntu / Debian

```bash
sudo apt update
sudo apt install -y btop curl wget unzip git neovim nano make python3 python3-pip python3-venv \
  lsd fd-find zoxide yazi dust bat fzf less openssh-server openssh-client ripgrep zsh
```

>   ⚠️ `fd`包名为 `fd-find`，`dust`和 `lazygit`需另行安装（见下方）。

#### Ubuntu 额外：lazygit & dust

```bash
# lazygit
sudo add-apt-repository ppa:lazygit-team/release
sudo apt update
sudo apt install -y lazygit

# dust (cargo 安装)
sudo apt install -y cargo
cargo install du-dust
```

### Termux (Android)

```bash
apt update
apt install btop curl wget unzip git neovim nano make python python-pip \
  lsd fd zoxide yazi bat fzf less openssh ripgrep zsh
```

>   ⚠️ Termux 无需 `sudo`，`fd`直接使用 `fd`包名，`dust`和 `lazygit`可通过 `cargo install`安装。

|      |      |
| ---- | ---- |
|      |      |
|      |      |
|      |      |
|      |      |
|      |      |
|      |      |
