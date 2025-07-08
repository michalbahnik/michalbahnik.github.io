# Thinkpad P14s - Ubuntu 22.04

This page documents installation and setup of Ubuntu 22.04 on Lenovo ThinkPad P14s Gen5 (21ME000DCK) with AMD processor adn integrated GPU.

## TL;DR

All went surprisingly fine.

## Instalation

* Following [official Lenovo document](https://download.lenovo.com/pccbbs/mobiles_pdf/ubuntu_20.04_lts_installation_v1.3_thinkpad.pdf) for BIOS setup and Ubuntu installation was without issues, even though it is for Ubuntu 22.04 - just minor discrepancies in BIOS setup.

## Setup

* GPU drivers installed using [official AMD installation guide](https://amdgpu-install.readthedocs.io/en/latest/index.html).
* Fingerprint scanner, microphone, speakers, camera etc. drivers work out-of-the-box (laptop hardware [certified](https://ubuntu.com/certified/202406-34087) to be Ubuntu compatible).
* Installed apps/utils:
  * `terminator`
  * `tmux`
  * `btop`
  * `docker`
  * `zsh` (`oh-my-zsh`) with `agnoster` theme
  * `fzf`
  * `baobab`
* Czech "coder" keyboard layout set up ([github repo](https://github.com/michalkahle/czech-coder-xkb)).
* Various tips from [linux_fu](https://github.com/michalbahnik/linux_fu/blob/main/README.md) applied.

## Update to Ubuntu 24.04

* Nothing got broken.
* GPU drivers reinstallation needed.
* Battery life subjectively improved.

## What worked (surprisingly) well

* All HW drivers (but fingerprint sensor, see below) work out of the box (wifi, mic, camera, bluetooth, ...). GPU driver was easy to install.
* Sleep mode uses reasonable amount of energy (< 1%/hour).

## What worked bad

* [ ] **Touchpad:** Touchpad gestures are limited, do not allow changing tabs/windows (3- vs 4-finger swipes).
* [ ] **Fingerprint:** After adding second user, no more fingerprints are possible to be added for any user. Using command line seems to help.
* [ ] **Monitor setup:** Monitor setup is not saved after restart and sometimes even after plug-out plug-in.
* [ ] **Icon stacking:** Some apps do not stack in dock, when added to favourites. Partially solved by creating _.desktop_ file.
