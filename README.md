# <p align="center">mangadesk - Terminal client for MangaDex 📖</p>

**<div align="center">Note: Repository is in maintenance mode. No new features will be worked on and will be postponed
to a later date.</div>**


<p align="center">
  <img alt="Top Language" src="https://img.shields.io/github/languages/top/darylhjd/mangadesk?style=flat-square">
  <img alt="License" src="https://img.shields.io/github/license/darylhjd/mangadesk?style=flat-square&color=blue">
  <img alt="Go Report" src="https://goreportcard.com/badge/github.com/darylhjd/mangadesk?style=flat-square">  
  <img alt="Downloads" src="https://img.shields.io/github/downloads/darylhjd/mangadesk/total?style=flat-square&color=success">
</p>

<p align="center">
  Download manga directly from your terminal to read!<br><br>
  <img src=".github/assets/demo.gif" alt="demo.gif">
</p>

<p align="center">
  This client retrieves information straight from MangaDex v5's API.<br>
  As the API is still a WIP, some changes (probably breaking) might be expected.
</p>

## Features ✨

- Download chapters straight to your computer.
- Login to keep track of your followed manga.
- Keep track of already downloaded manga.
- Download multiple chapters together.
- Searching!
- Responsive UI (kind of)
- Written in Golang :)

Works for Windows/Linux/macOS.

## Installation 🔧

This application runs as a standalone executable, and does not need to be installed.

Check out the [Releases Page](https://github.com/darylhjd/mangadesk/releases) for new releases. To update, just
download the latest release.

For bleeding edge 🗡 updates, you may also compile from source:

```cmd
$ git clone https://github.com/darylhjd/mangadesk.git
$ cd mangadesk
$ go get -d ./...
$ go build
```

### Arch Linux

Mangadesk is available through the [AUR](https://aur.archlinux.org/packages/mangadesk/) and may be installed as such (thanks @AmaanHUB!). 
It may be installed manually or with your preferred AUR helper:

```cmd
$ paru -S mangadesk
```

## Uninstall ❌

To uninstall, simply delete the executable and its related folders and files (namely, the `usr` folder).

Your downloads will not be removed by deleting the executable.

### Arch Linux

Uninstall with an AUR helper or with pacman:

```cmd
$ pacman -R mangadesk
```

## Usage ✍

To run the application, navigate to the directory where you stored the executable, and run the following command:

```cmd
$ ./mangadesk 
```

Steps may differ for different OSes. For example, in Windows, use a backslash `\` instead.

### Keybindings ⌨

| Operation                 | Binding                          | Page       |
|---------------------------|----------------------------------|------------|
| Login/Logout              | <kbd>Ctrl</kbd> + <kbd>L</kbd>   | All        |
| Keybindings/Help          | <kbd>Ctrl</kbd> + <kbd>K</kbd>   | All        |
| Search                    | <kbd>Ctrl</kbd> + <kbd>S</kbd>   | All        |
| Next/Prev Page            | <kbd>Ctrl</kbd> + <kbd>F/B</kbd> | Some       |
| Escape                    | <kbd>Esc</kbd>                   | Some       |
| Select multiple chapters  | <kbd>Ctrl</kbd> + <kbd>E</kbd>   | Manga Page |
| Toggle select all         | <kbd>Ctrl</kbd> + <kbd>A</kbd>   | Manga Page |

## Settings ⚙

Refer to [this document](app/core/CONFIG.md) for configurable settings.

## Issues ☠

Check out the Issues page for current issues/feature requests.

## Contributing 🤝

Always welcome and appreciated :)

Please take some time to familiarise yourself with the [contributing guidelines](.github/CONTRIBUTING.md).

## Learning Points 🧠

- Creating TUIs with tview/tcell.
- Working with the filesystem in Golang.
- Goroutines & Context.
- Go Project structure.
