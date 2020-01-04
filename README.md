Arpit's Python with randomizing addition operator
==================================================

This version of python has addition operator gone rogue. When asked to add
two variable it performs one of subtraction, multiplication, division and power function
at random. To know more details about what, why and how I recommend you
checkout my blog post
[arpitbhayani.me/blogs/i-changed-my-python](https://arpitbhayani.me/blogs/i-changed-my-python).


                              @.
                           @@@     @@@@@@@
                         @@@@@@@@@@@@@@@@@@@@@@@@@
                   .@% %@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
                  @@@ @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@(
                 @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
               ,@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
               @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
              @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
              @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@(
             @@@@@@@@@@@@@@%       *@@@@@@@@@@@@@@@@@@@@@@@@@
             @@@@@@@@@@@@                @@@@@@@@@@@@@@@@@@@@@
             @@@@@@@@@@                           @@@@@@@@@@@@@
             @@@@@@@@@                               &@@@@@@@@@@@
             @@@@@@@@                                  @@@@@@*
             (@@@@@@@                                   @@@@@
              @@@@@@                                    @@@@@
              *@@@@@                                    @@@@@
               @@@@,                                    @@@@@
                @@@                                     @@@&
                 *@                                     @@
                  @                                     #


This repository is forked from Python version 3.9.0 alpha 2; then what makes this different?

In order to understand the internals of Python, I override the addition operator `+`
(where at least one of the two operands should be a variable) such that
it picks one of the following operators `+`, `-`, `*`, `/`, `**` at random and applies it on the
given operands. See it in action below

![Python Internals - Overriding addition operator](https://user-images.githubusercontent.com/4745789/71643972-d96b2780-2ce6-11ea-894c-fd638dc95d7c.gif)

Although it does not have make sense to have such a behavior but it makes a good first exercise
to understand the internals of Python language.

## Setup and building the executable

Execute following set of commands that will build the executable `python.exe` from the source

```
./configure
make
```

Once both of above commands are executed successfully then you will find an executable named
`python.exe` in your current directory. Executing this binary will start the Python shell built
from the source. Making any change in source code and running `make` will rebuild this binary.

```
./python.exe
```

## Troubleshooting

If you encounter any SSL issue please refer [TROUBLESHOOTING.md](https://github.com/arpitbbhayani/cpython/blob/01-randomized-math-operators/TROUBLESHOOTING.md)
file where steps to fix the SSL issue are mentioned. If you encounter any other issue then
Stackoverflow is your friend.
