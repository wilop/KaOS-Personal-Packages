# KaOS-Personal-Packages
This is my KaOS personal packages repository.  
All packages are built and tested by myself before pushing them to [KaOS-Community-Packages](https://github.com/KaOS-Community-Packages).  


## Packages
This repository contains the following packages:  
  - [android-tools](https://github.com/wilop/android-tools)  
  - [arduino-ide](https://github.com/wilop/arduino-ide)  
  - [vendetta-online](https://github.com/wilop/vendetta-online)  
  - [fastfetch](https://github.com/wilop/fastfetch)  
  - [rt3290-dkms](https://github.com/wilop/rt3290-dkms.git)  

## Installation
  - ### In kcp
  Run in command line `kcp -i package`; replace `package` with the package you want to install, e.g:
  
  ```bash
  kcp -i fastfetch
  ```

  - ### Not in kcp
  Clone the package repository, e.g:
  
  ```bash
  git clone https://github.com/wilop/fastfetch.git
  ```
  
  Then use `makepkg` to build the package and `pacman` to install it, e.g:
  
  ```bash
  cd fastfetch
  makepkg -s --check --clean
  sudo pacman -U fastfetch-2.49.0-1-x86_64.pkg.tar.zst
  ```
  
## How to clone
> _Packages are organized in a set of git submodules_.  

To  clone this repository, use the following command:  

```bash
git clone https://github.com/wilop/KaOS-Personal-Packages.git
```

To init the submodules, use the following commands into each submodule:  

```bash
git submodule init
git submodule update
```

To clone this repository with all submodules, use the following command:  

```bash
git clone --recursive https://github.com/wilop/KaOS-Personal-Packages.git
```
