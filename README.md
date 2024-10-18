# all_things_BASH
Notes from the Book Black Hat Bash

Notes:
https://google.github.io/styleguide/shellguide.html

The shebang line

Standard:
  #!/bin/bash

Portable:
  #!/usr/bin/env bash

Prints all commands and thier arguments as the are exectued to the terminal:
  #!/bin/bash -x

To run script w/o shebang:
  bash helloworld.sh

To dry run script for debug
  bash -n helloworld.sh

Can run in verbose mode
  bash -x helloworld.sh

Set debug areas
  #!/bin/bash
  set -x
  #----snip---
  set +x


  #VARIABLES
  book="black hat bash"
    echo $book
        or
    echo ${book}

root@kali:~# root_directory=$(ls -ld /)
root@kali:~# echo "${root_directory}" 
root@kali:~# drwxr-xr-x 23 root root 4096 Oct 18 18:36 /


