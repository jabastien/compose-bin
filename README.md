# compose-bin #

## Description ##

Common shell scripts for managing docker and docker-compose projects.
Generally included as a submodule of other projects.

## Installing ##
https://github.com/blog/2104-working-with-submodules
```bash
$ cd /main/project
$ git submodule add -b master git@github.com:klutchell/compose-bin.git bin
$ git commit -m "compose-bin submodule"
$ git submodule update --init --recursive
```

## Usage ##
The submodule is its own repo/work-area, with its own .git directory.
So, first commit/push your submodule's changes:
```bash
$ cd path/to/submodule
$ git add <stuff>
$ git commit -m "comment"
$ git push
```

Then tell your main project to track the updated version:
```bash
$ cd /main/project
$ git add path/to/submodule
$ git commit -m "updated my submodule"
$ git push
```

## Contributing ##

n/a

## Author ##

Kyle Harding <kylemharding@gmail.com>

## Credit ##

n/a