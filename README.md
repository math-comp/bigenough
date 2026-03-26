<!---
This file was generated from `meta.yml`, please do not edit manually.
Follow the instructions on https://github.com/coq-community/templates to regenerate.
--->
# bigenough

[![Docker CI][docker-action-shield]][docker-action-link]

[docker-action-shield]: https://github.com/math-comp/bigenough/actions/workflows/docker-action.yml/badge.svg?branch=master
[docker-action-link]: https://github.com/math-comp/bigenough/actions/workflows/docker-action.yml




The package contains a package to reasoning with big enough objects
(mostly natural numbers). This package is essentially for backward
compatibility purposes as `bigenough` will be subsumed by the near
tactics. The formalization is based on the Mathematical Components
library.

## Meta

- Author(s):
  - Cyril Cohen
- License: [CeCILL-B](LICENSE)
- Compatible Rocq/Coq versions: 8.10 or later
- Additional dependencies:
  - [MathComp boot](https://math-comp.github.io) 1.6 or later (MathComp ssreflect for versions <= 2.4.0)
- Rocq/Coq namespace: `mathcomp.bigenough`
- Related publication(s): none

## Building and installation instructions

The easiest way to install the latest released version of bigenough
is via [OPAM](https://opam.ocaml.org/doc/Install.html):

```shell
opam repo add rocq-released https://rocq-prover.org/opam/released
opam install rocq-mathcomp-bigenough
```

To instead build and install manually, you need to make sure that all the
libraries this development depends on are installed.  The easiest way to do that
is still to rely on opam:

``` shell
git clone https://github.com/math-comp/bigenough.git
cd bigenough
opam repo add rocq-released https://rocq-prover.org/opam/released
opam install --deps-only .
make   # or make -j <number-of-cores-on-your-machine> 
make install
```


# A small library to do epsilon - N reasoning.

This repository is essentially for archiving purposes as `bigenough`
will be subsumed by the [near tactics](https://github.com/math-comp/analysis/blob/9bfd5a1971c6989f51d9c44341bb71b2fd5e3c76/topology.v#L93).

The formalization is based on the [Mathematical Components](https://github.com/math-comp/math-comp) library for the [Coq](https://coq.inria.fr) proof assistant,
although it requires only the boot package.
