# OCaml
Repository for learning OCaml

Steps used to install OCaml and run a basic HelloWorld program.
 
  sudo apt-get install ocaml
  
  sudo add-apt-repository ppa:avsm/ppa
  
  sudo apt-get update
  
  sudo apt-get install ocaml-native-compilers calmp4-extra opam
  
  sudo apt-get install ocaml-native-compilers camlp4-extra opam
  
  Take it for a spin ... 
  
  opam
  
  opam list
  
  opam init
  
  eval `opam config env`
  
  ocaml
  
  create an OCaml directory ... 
  
  mkdir OCaml
  
  cd OCaml
  
  Compile a file
  
  ocamlc -o hello hello.ml
  
  Execute the compiled program
  
  ./hello
  
  -------------------------------------------------------------------------------------------------------------------
  The book Real World OCaml: Functional Programming for the Masses by Yaron Minsky, Anil Madhavapeddy & Jason Hickey,
  uses Core, a library from Jane Street Capital.  

  One could download Core from Jane Street Capital's GitHub (https://github.com/janestreet/core) but I don't now how
  this should be installed.  The package manager OPAM handles the installation better.  To install using OPAM, type:
  
  opam install core
  
  -------------------------------------------------------------------------------------------------------------------
  Additional OPAM download that are needed to follow the example in the book:
  
  opam install utop
  opam install async
  
  -------------------------------------------------------------------------------------------------------------------
  
  Create .ocamlinit
  
  From Linux shell, open your favorite editor and create the file .ocamlinit
  Add the following content:

#use "topfind"
#thread
#require "ppx_jane,core.top"
#require "async"
#require "core.extended"
open Core.Std

  -------------------------------------------------------------------------------------------------------------------
Explanation of the bug with .ocamlinit

File ".ocamlinit", line 1:
Error: Reference to undefined global `Longident'

https://github.com/diml/utop/issues/213

  -------------------------------------------------------------------------------------------------------------------
  Good resources:
  
  https://realworldocaml.org/
  
  http://www.cs.cornell.edu/courses/cs3110/2018sp/
  
  https://caml.inria.fr/pub/docs/u3-ocaml/ocaml-steps.html
  
  
  
