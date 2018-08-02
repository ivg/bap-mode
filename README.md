# bap-mode: an Emacs major mode for BAP's intermediate representation

## What is bap-mode?

bap-mode is an Emacs major mode for reading and analyzing programs in [BAP](https://github.com/BinaryAnalysisPlatform/bap)'s IR. It allows to interact with BAP from within emacs. For example, *bap-open-file* (`C-c o`) opens a file with BAP and emits the IR to an Emacs buffer. bap-mode hightlights the syntax and allows to quickly navigate the code (e.g. `C-c m` to jump to the main function).

## How to install bap-mode?

bap-mode is avilable on [Melpa](https://melpa.org/). Install it with M-x package-install <RET> bap-mode <RET>.

## How to use bap-mode?

The following keybindings are defined per default:
- `C-c d` *bap-goto-function-definition*: jump to a function definition
- `C-c l` *bap-goto-label*: jump to a label
- `C-c m` *bap-goto-main*: jump to main function
- `C-c o` *bap-open-file*: opens a binary with BAP and emits the IR
- `C-c p` *bap-open-file-with-extra-pass*: same as above but adds an extra pass before emitting the IR

## Future work

Some of the things that would be nice to have are:
- helm support for better navigation
- jump to definition at point

As always on github, pull requests are welcomed!

## Acknowledgments
This project is partly financed by [German Federal Office for Information Security (BSI)](https://www.bsi.bund.de). 

## License
```
    The MIT License (MIT)

    bap-mode
    Copyright (C) 2018 Thomas Barabosch of Fraunhofer FKIE
    
    Based on emacs-mips-mode
    Copyright (c) 2017 Henrik Lissner
    
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
    the following conditions:

    The above copyright notice and this permission notice shall be
    included in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
    IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
    CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
    TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
    SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```