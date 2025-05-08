[![x86_64-ubuntu24](https://github.com/user4223/pacman/actions/workflows/x86_64_ubuntu24.yml/badge.svg)](https://github.com/user4223/pacman/actions/workflows/x86_64_ubuntu24.yml)

# What's this for?
Minimal project template using cpp, cmake, conan and gtest.
Replace all occurrences of 'Pacman' and 'pacman' in file names,
scripts and source files by your desired application name and
use it as a base for your cpp-project having dependency management,
build system and ci pipeline configured properly (at time of writing).
ftxui is used as sample dependency here, take a look on all occurrences
of 'ftxui' in cmake files, sources and conanfile and replace by dependencies
you need for your project.

# Instructions on Ubuntu

## Initial Setup
It assumes you have a modern python3 and venv module installed already. Otherwise you might need `apt-get install --no-install-recommends -y python3-venv` as well.
```
apt-get install --no-install-recommends -y build-essential make cmake

python3 -m venv venv
. venv/bin/activate

pip install conan
```

## Build for Development
```
./build.sh Debug -- -j
```

# Instructions on MacOS

## Initial Setup
```
xcode-select --install

brew install cmake make        # Maybe some other dev-tools as well...

python3 -m venv venv
. venv/bin/activate

pip install conan
```

## Build for Development
```
./build.sh Debug -- -j
```