# kif445-lisp-tutorial
This project is meant to introduce the Konferenz der Informatikfachschaften to Common-Lisp.

##Install Emacs with the SBCL compiler

https://gist.github.com/jteneycke/7947353

Console:
* sudo apt-get install emacs
* sudo apt-get install sbcl
* curl -O http://beta.quicklisp.org/quicklisp.lisp
* sbcl --load quicklisp.lisp

Now in the SBCL context:
* (quicklisp-quickstart:install)
* (ql:quickload "quicklisp-slime-helper")

Quicklisp in Emacs einbinden:
* echo "(load (expand-file-name "~/quicklisp/slime-helper.el"))" > ~/.emacs
Replace "sbcl" with the path to your implementation
* echo "(setq inferior-lisp-program "/usr/bin/sbcl")" >> ~/.emcas