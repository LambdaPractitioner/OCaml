# OCaml
Repository for learning OCaml

Steps used to install OCaml and run a basic HelloWorld program.  Numbers are just history on my particular machine.

  640  ocaml
  
  641  sudo apt-get install ocaml
  
  642  opam
  
  643  sudo add-apt-repository ppa:avsm/ppa
  
  644  sudo apt-get update
  
  645  sudo apt-get install ocaml-native-compilers calmp4-extra opam
  
  646  sudo apt-get install ocaml-native-compilers camlp4-extra opam
  
  647  opam
  
  648  opam list
  
  649  opam init
  
  650  eval `opam config env`
  
  651  ocaml
  
  652  ls
  
  653  mkdir OCaml
  
  654  cd OCaml
  
  655  ls
  
  656  ocamlc -o hello hello.ml
  
  657  ./hello
  
  -------------------------------------------------------------------------------------------------------------------
  
  Download Core from Jane Street Capital's GitHub.
  https://github.com/janestreet/core
  
  Better is just installing using OPAM
  
  opam install core
  
  -------------------------------------------------------------------------------------------------------------------
  
  opam install utop
  opam install async
  
  -------------------------------------------------------------------------------------------------------------------
  
  Create .ocamlinit
  
  From Linux shell, open your favorite editor and create the file .ocamlinit
  Add the following content:

#use "topfind"
#thread
#require "ppx jane,core.top"
#require "async"
#require "core.extended"
open Core.Std

  -------------------------------------------------------------------------------------------------------------------
  
  http://www.cs.cornell.edu/courses/cs3110/2018sp/
  
  https://caml.inria.fr/pub/docs/u3-ocaml/ocaml-steps.html
  
  https://realworldocaml.org/
  
