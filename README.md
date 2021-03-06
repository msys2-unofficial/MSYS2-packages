# MSYS2-packages-unofficial

[![Sponsor](https://img.shields.io/badge/Support%20Me-%F0%9F%92%97-ff69b4.svg)](https://www.patreon.com/DamonKwok)
<!-- [![Gitter chat][1]][2]&nbsp;&nbsp; -->
<!-- [![AppVeyor status][3]][4]&nbsp;&nbsp; -->
<!-- [![Azure status][5]][6]&nbsp;&nbsp; -->

[1]: https://badges.gitter.im/msys2/msys2.png
[2]: https://gitter.im/msys2/msys2
[3]: https://ci.appveyor.com/api/projects/status/github/Alexpux/MSYS2-packages?branch=master&svg=true
[4]: https://ci.appveyor.com/project/Alexpux/MSYS2-packages
[5]: https://dev.azure.com/msys2/mingw/_apis/build/status/msys2.MSYS2-packages?branchName=master&svg=true
[6]: https://dev.azure.com/msys2/mingw/_build/latest?definitionId=5&branchName=master

<img src="https://raw.githubusercontent.com/msys2-unofficial/MSYS2-packages/master/msys2.png" alt="MSYS2" title="it's cool!" />
 
Package scripts for MSYS2.

To build these, run <label style="color:green">**msys2_shell.cmd**</label> then from the bash prompt. Packages from
the **msys2-devel** and **base-devel** groups are implicit build time dependencies.
Make sure both are installed before attempting to build any package:

    pacman -S --needed base-devel msys2-devel
    cd ${package-name}
    makepkg -sf

To install the built package(s).

    pacman -U ${package-name}*.pkg.tar.xz
    
For example

build [mu](mu/README.org)

## Official packages

[Home](https://www.msys2.org/)
[msys2/MSYS2-packages](https://github.com/msys2/MSYS2-packages)

## License

MSYS2-packages-unofficial is licensed under BSD 3-Clause "New" or "Revised" License.
A full copy of the license is provided in [LICENSE](LICENSE).
