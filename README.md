# GameDie
[![C/C++ CI](https://github.com/NoahIles/GameDie/actions/workflows/c-cpp.yml/badge.svg)](https://github.com/NoahIles/GameDie/actions/workflows/c-cpp.yml)

This repository provides a class that represents a game die, such as the
six-sided dice used in traditional dice game. While the die defaults to 
six sides, the overloaded constructor allows the developer to customize
any size die (with at least one face). It also keeps track of how many
times a certain face has been rolled so that the fairness of the die
can be examined.

## Getting Started

Build the image from `Dockerfile` with the command:

`docker build -t cpp-container .`

Once built, run the image:

`docker run -it cpp-container`

...or run it interactively in a shell:

`docker run -it cpp-container sh`

...or run it with a bind mount to the current source code:

`docker run --mount type=bind,source="$(pwd)",target=/usr/src -it cpp-container`