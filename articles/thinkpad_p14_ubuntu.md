# Thinkpad P14s - Ubuntu 22.04

This page documents installation and setup of Ubuntu 22.04 on Lenovo ThinkPad P14s Gen5 (21ME000DCK) with AMD processor.

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
* Czech "coder" keyboard layout set up ([github repo](https://github.com/michalkahle/czech-coder-xkb)).

# Unresolved issues

* [] 
