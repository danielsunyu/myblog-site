+++
title = 'Run xv6-x86-64 on macOS M'
date = 2026-03-05T21:41:33-07:00
draft = false
+++

https://en.wikipedia.org/wiki/Xv6

I used to believe it's not possible to run `xv6-x86-64` version on macOS with arm chip. It turns out that it is not 
that hard to do that with `qemu`.

All we need is to install `qemu` on your macOS.

```zsh
brew install qemu
```

Verify:
```zsh
which qemu-system-x86_64
$ /opt/homebrew/bin/qemu-system-x86_64
```

Install cross-compilation toolchain:
```zsh
$ brew install x86_64-elf-gcc
$ which x86_64-elf-gcc
$ /opt/homebrew/bin/x86_64-elf-gcc
```

```bash
make qemu-nox   
```

