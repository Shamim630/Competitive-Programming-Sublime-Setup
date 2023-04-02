# Competitive-Programming-Sublime-Setup
This setup will make your CP faster, no need to input data manually to the prompt again and again, code input and output will be in a single window.

 <p align="center">Get dynamically generated GitHub stats!</p>

<p align="center">
  <a href="https://github.com/vividblueprint/Competitive-Programming-Sublime-Setup/actions">
    <img alt="Tests Passing" src="https://github.com/anuraghazra/github-readme-stats/workflows/Test/badge.svg"/>
  </a>
  <a href="https://github.com/vividblueprint/Competitive-Programming-Sublime-Setup/contributors">
    <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/vividblueprint/Competitive-Programming-Sublime-Setup"/>
  </a>
  <a href="https://github.com/vividblueprint/Competitive-Programming-Sublime-Setup/issues">
    <img alt="Issues" src="https://img.shields.io/github/issues/vividblueprint/Competitive-Programming-Sublime-Setup?color=0088ff"/>
  </a>
  <a href="https://github.com/vividblueprint/Competitive-Programming-Sublime-Setup/pulls">
    <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/vividblueprint/Competitive-Programming-Sublime-Setup?color=0088ff">
  </a>
  <br />
<img alt="Lines of code" src="https://img.shields.io/tokei/lines/github/vividblueprint/Competitive-Programming-Sublime-Setup?color=green">
<img alt="GitHub language count" src="https://img.shields.io/github/languages/count/vividblueprint/Competitive-Programming-Sublime-Setup?color=302df0">
<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/vividblueprint/Competitive-Programming-Sublime-Setup">
<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/vividblueprint/Competitive-Programming-Sublime-Setup?color=0088ff">
<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/vividblueprint/Competitive-Programming-Sublime-Setup?color=00ff00f">
<img alt="GitHub repo file count" src="https://img.shields.io/github/directory-file-count/vividblueprint/Competitive-Programming-Sublime-Setup">
</p>

# Table of Contents
1. [Install MSYS2](#install-msys2)
1. [Install the G++ and G++ Compilers](#install-the-g-and-g-compilers)
1. [Install the Debugger](#install-the-debugger)
1. [Add the Directory to the Path of the Environment Variables](#add-the-directory-to-the-path-of-the-environment-variables)
1. [Check the Install](#check-the-install)

## Install MSYS2
At first download the executable file from MSYS2. Go to the official website of MSYS2: https://www.msys2.org/
Scroll-down a little bit until you find the download button for the executable file.
1. `Download and install the exeicutable.`
1. `Wait untill installation is completed.`
1. `Open MSYS2 MSYS terminal`
1. `Apply the command below to update the package database and the base packages:`

        pacman -Syu
1. `Reopen the MSYS2 MSYS terminal and apply the command below`

        pacman -Su
        pacman -Sy

## Install the G++ and G++ Compilers
If you are using a 64 bit operating system
then open `MSYS2 MinGW x64` terminal and execute the command below:

        pacman -S mingw-w64-x86_64-gcc 

⚠️ if you are using a 32 bit operatiog system then open `MSYS2 MinGW x86` terminal and execute the command below:

        pacman -S mingw-w64-i686-gcc

## Install the Debugger
If you are using a 64 bit operating system then execute the command below on `MSYS2 MinGW x64` terminal :

        pacman -S mingw-w64-x86_64-gdb

⚠️ If you are using a 32 bit operating system then execute the command below on `MSYS2 MinGW x86` terminal :

        pacman -S mingw-w64-i686-gdb

## Add the Directory to the Path of the Environment Variables

Click on windows button and search `Environment Variables` then open it.

1. If you are using a 64 bit operating system, then go to `mingw64 > bin` folder from `C:\` directory and copy the path or copy the path from below:

        C:\msys64\mingw64\bin

    ⚠️ If you are using a 32 bit operating system, then go to `mingw32 > bin` folder from `C:\` directory and copy the path or copy the path from below:

        C:\msys64\mingw32\bin

1. Click on `Path`, click `Edit`, add a   `new` path and Paste coppied directory here. Click `OK`.

## Check the Install
Open the terminal / PowerShell / CMD and apply the commands serially:

1. check for the `GCC` version:

        gcc --version
        
1. check for the `G++` version:

        g++ --version
1. check for the `GDB` version:

        gdb --version

At last, install [`sublime text editor`](https://www.sublimetext.com/download) and copy these `build` files to the `sublime text editor`'s `tool` option directory. Select a `build` file from the `tool` option and enjoy your `CP`.