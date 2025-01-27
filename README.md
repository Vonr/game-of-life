# Conway's Game of Life

## Introduction

### Conway's Game of Life in an many programming languages as I can figure out

![Ada](https://img.shields.io/badge/ada-%230000AA.svg?style=for-the-badge)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=.net&logoColor=white)
![D](https://img.shields.io/badge/d-%2398312A.svg?style=for-the-badge&logo=d&logoColor=white)
![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![F#](https://img.shields.io/badge/f%23-%2330B9DB.svg?style=for-the-badge&logo=.net&logoColor=white)
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![Haskell](https://img.shields.io/badge/Haskell-5e5086?style=for-the-badge&logo=haskell&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Julia](https://img.shields.io/badge/-Julia-9558B2?style=for-the-badge&logo=julia&logoColor=white)
![Lua](https://img.shields.io/badge/lua-%232C2D72.svg?style=for-the-badge&logo=lua&logoColor=white)
![Nim](https://img.shields.io/badge/nim-%23FFE953.svg?style=for-the-badge&logo=nim&logoColor=black)
![Perl](https://img.shields.io/badge/perl-%2339457E.svg?style=for-the-badge&logo=perl&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-%235391FE.svg?style=for-the-badge&logo=powershell&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Ruby](https://img.shields.io/badge/ruby-%23CC342D.svg?style=for-the-badge&logo=ruby&logoColor=white)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Visual Basic](https://img.shields.io/badge/visual_basic-%2368217a.svg?style=for-the-badge&logo=.net&logoColor=white)
![Zig](https://img.shields.io/badge/Zig-%23F7A442.svg?style=for-the-badge&logo=zig&logoColor=black)

<!--
![Assembly](https://img.shields.io/badge/Assembly-black?style=for-the-badge&logo=arm&logoColor=white)
![Forth](https://img.shields.io/badge/forth-%23EF5350.svg?style=for-the-badge)
![Elixir](https://img.shields.io/badge/elixir-%234B275F.svg?style=for-the-badge&logo=elixir&logoColor=white)
![Fortran](https://img.shields.io/badge/Fortran-%23734F96.svg?style=for-the-badge&logo=fortran&logoColor=white)
-->

The games are all setup to run a 100x50 (WxH) board for 500 generations. Most of them were originally written to be dynamic and find the terminal
size or accept arguments but it was taking too much work to get all of that set up for each language and (imo) distracting from the purpose of this
by shifting half of the work onto random argument parsing libraries rather than the languages themselves.

## Contents

- [Prerequisites](#prerequisites)
- [Build From Source](#build-from-source)
- [Benchmarking](#benchmarking)
- [Container Build](#container-build)
- [Visual Studio Code Dev Container](#dev-container)

## Prerequisites

<!--
- Assembly
  - GNU Binutils (as & ld)
  - Raspberry Pi 4
- Elixir
- Fortran
  - GCC (gfortran)
-->
- Ada 95
  - GCC Gnat
  - GCC Gnatmake
- Bash
- C
  - GCC
  - GNU Make
- C++
  - GCC
  - Meson
  - Ninja
- C#
  - .NET 7.0 SDK
- D
  - GCC GDC
- Dart
- F#
  - .NET 7.0 SDK
- Go
- Haskell
  - GHC
- Java
  - Gradle
- Julia
- Lua
- Nim
- Perl
- PowerShell
- Python
- Ruby
- Rust
  - Cargo
- Typescript
  - Node.js
  - Yarn
- Visual Basic
  - .NET 7.0 SDK
- Zig

## Build from Source

<!-- ### Assembly

This is written for a Raspberry Pi 4 running aarch64 Linux

```sh
cd asm/
make
./game_of_life
``` -->

### Ada

```sh
cd ada/
gnatmake src/game_of_life.adb
./game_of_life
```

### Bash

```sh
cd bash/
./game_of_life.sh
```

### C

```sh
cd c/
make
./game_of_life
```

### C++

```sh
cd cpp/
meson setup build
cd build
ninja
./game_of_life
```

### C\#

```sh
cd csharp/
dotnet run
```

### D

```sh
cd d/
make
./game_of_life
```

### Dart

```sh
cd dart/
dart run
```

<!-- ### Elixir

```sh
cd elixir/
elixir game_of_life.exs
``` -->

### F\#

```sh
cd fsharp/
dotnet run
```

### Go

```sh
cd go/
go run .
```

### Haskell

```sh
cd haskell/
ghc -o game_of_life main.hs game.hs board.hs
./game_of_life
```

### Java

```sh
cd java/
./gradlew run --console plain
```

### Julia

```sh
cd julia/
julia game_of_life.jl
```

### Lua

```sh
cd lua/
lua game_of_life.lua
```

### Nim

```sh
cd nim/
nim c -r GameOfLife.nim
```

### Perl

```sh
cd perl/
perl GameOfLife.pl
```

### PowerShell

```sh
cd powershell/
pwsh Game-Of-Life.ps1
```

### Python

```sh
cd python/
python game_of_life.py
```

### Ruby

```sh
cd ruby/
ruby GameOfLife.rb
```

### Rust

```sh
cd rust/
cargo run
```

### Typescript

```sh
cd typescript/
yarn install
yarn run start
```

### Visual Basic

```sh
cd vb/
dotnet run
```

### Zig

```sh
cd zig/
zig build run
```

## Benchmarking

There's an included script to build all version and run benchmarks. It requires [zx](https://github.org/google/zx) to run

```sh
zx --install benchmark.mjs
```

`--install` is only needed on the first run to install the script's dependencies

You can also specify how many iterations to run the benchmark (default 5), averaging the results

```sh
./benchmark.mjs --iterations 5
```

The set of languages to run in the benchmark can also be set. NOTE: Some languages, e.g. bash, powershell, are disabled by default for performance reasons. The default set is "ada,c,cpp,csharp,d,dart,fsharp,go,haskell,java,julia,lua,nim,perl,python,ruby,rust,typescript,vb,zig"

```sh
./benchmark.mjs --languages c,cpp,rust
# of
./benchmark.mjs --languages all
```

## Container Build

```sh
podman build -t game-of-life .

podman run --rm game-of-life
# or
podman run --rm game-of-life --iterations 5 --languages c,cpp,rust
```

> NOTE: Docker will also work

## Prebuilt Container

[![Container build](https://github.com/mrivnak/game-of-life/actions/workflows/publish-image.yml/badge.svg)](https://github.com/mrivnak/game-of-life/actions/workflows/publish-image.yml)

There's a prebuilt image on GitHub Container Registry since the container build is quite long, especially on low powered systems. Images will be available for x86_64 and aarch64. riscv64 will also be available once software support is available

```sh
podman pull ghcr.io/mrivnak/game-of-life:main
podman run --rm mrivnak/game-of-life:main
```

## Dev Container

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

Provided is a `devcontainer.json` file that will automatically setup a development environment for all of the languages in here, along with relevant extensions and language servers
