dockerfile — Library for manipulating Dockerfiles
-------------------------------------------------------------------------------
%%VERSION%%

[Docker](http://docker.com) is a container manager that can build images
automatically by reading the instructions from a `Dockerfile`. A Dockerfile is
a text document that contains all the commands you would normally execute
manually in order to build a Docker image. By calling `docker build` from your
terminal, you can have Docker build your image step-by-step, executing the
instructions successively.  Read more at <http://docker.com>

This library provides a typed OCaml interface to generating Dockerfiles
programmatically without having to resort to lots of shell scripting and
awk/sed-style assembly.

dockerfile is distributed under the ISC license.

Homepage: https://github.com/avsm/ocaml-dockerfile  
Contact: Anil Madhavapeddy `<anil@recoil.org>`

## Installation

dockerfile can be installed with `opam`:

    opam install dockerfile

If you don't use `opam` consult the [`opam`](opam) file for build
instructions.

## Documentation

The documentation and API reference is automatically generated by
`ocamldoc` from the interfaces. It can be consulted [online][doc]
and there is a generated version in the `doc` directory of the
distribution.

[doc]: https://anil-code.recoil.org/ocaml-dockerfile/doc

## Sample programs

If you installed dockerfile with `opam` sample programs are located in
the directory `opam config var dockerfile:doc`.

In the distribution sample programs and tests are located in the
[`test`](test) directory of the distribution. They can be built with:

    ocamlbuild -use-ocamlfind test/tests.otarget

The resulting binaries are in `_build/test`.

- `test.native` tests the library, nothing should fail.
