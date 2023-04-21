<!-- HEADERS -->
<p align="center">
  <b> ~ Mauwu's terminal configuration files ~ </b>
</p>

<!-- INFORMATION -->


<img src="https://raw.githubusercontent.com/mauriciocruzp/terminal/main/Mauwu'sTerminal.png" alt="img" align="right" width="400px">

This is my personal terminal configuration files.


The [setup section](#setup) will guide you through the installation process.

Here are some details about my setup:

- **WM:** [Mutter](https://gitlab.gnome.org/GNOME/mutter)
- **OS:** [Manjaro](https://manjaro.org/)
- **Terminal:** [kitty](https://github.com/kovidgoyal/kitty)
- **Shell:** [zsh](https://wiki.archlinux.org/index.php/Zsh)

---

<!-- SETUP -->

## Setup.

> This is step-by-step how to install these bspwm dotfiles. Just [R.T.F.M](https://en.wikipedia.org/wiki/RTFM).

### Installation (Manual)

> After cloning the repository, install the necessary dependencies to replicate by setup.

   <details open>
   <summary><strong>Arch Linux (and Arch-based distributions)</strong></summary>

> Assuming your **AUR Helper** is [yay](https://github.com/Jguer/yay).

```sh
 $ yay -S kitty lsd bat

```

   </details>

   <br>

> Then after the dependencies are installed, copy the files to it's respective folders.

   <details open>
   <summary><strong>Config</strong></summary>

```sh
 $ mkdir -p $HOME/.config/kitty && cp -r ./config/kitty/* $HOME/.config/kitty
 $ cp -r ./zsh/.zshrc $HOME/
```

   </details>

   <br>

> You will need to install this font.

- **HackNerdFont:** [here](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.3.3/Hack.zip)
   <br>

> Once finished copying the files, you might want to finalize the changes to your system.

```sh
 # Rebuilds the font cache
 $ fc-cache -fv
```

   <br>

> Lastly, log out from your current desktop session and log in into bspwm.

   <br>
