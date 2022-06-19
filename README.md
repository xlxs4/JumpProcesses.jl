# DiffEqJump.jl

[![Join the chat at https://gitter.im/JuliaDiffEq/Lobby](https://badges.gitter.im/JuliaDiffEq/Lobby.svg)](https://gitter.im/JuliaDiffEq/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Build Status](https://github.com/SciML/DiffEqJump.jl/workflows/CI/badge.svg)](https://github.com/SciML/DiffEqJump.jl/actions?query=workflow%3ACI)
[![Coverage Status](https://coveralls.io/repos/github/SciML/DiffEqJump.jl/badge.svg?branch=master)](https://coveralls.io/github/SciML/DiffEqJump.jl?branch=master)
[![codecov.io](https://codecov.io/gh/SciML/DiffEqJump.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/SciML/DiffEqJump.jl)
[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](http://jump.sciml.ai/stable/)
[![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](http://jump.sciml.ai/dev/)

DiffEqJump.jl provides methods for simulating jump processes, known as
stochastic simulation algorithms (SSAs), Doob's method, Gillespie methods, or
Kinetic Monte Carlo methods across different fields of science. It also enables the
incorporation of jump processes into hybrid jump-ODE and jump-SDE models,
including jump diffusions.

DiffEqJump is a component package in the [SciML](https://sciml.ai/) ecosystem,
and one of the core solver libraries included in
[DifferentialEquations.jl](https://github.com/JuliaDiffEq/DifferentialEquations.jl).

The documentation includes
- [a tutorial and details on using DiffEqJump to simulate jump processes via SSAs (i.e. Gillespie methods)](https://jump.sciml.ai/latest/discrete_stochastic_example/),
- [a reference on the types of jumps and available simulation methods](https://diffeq.sciml.ai/latest/jump_types/),
- [a FAQ](https://diffeq.sciml.ai/latest/faq.md) with information on changing parameters between simulations and using callbacks.

## Installation
There are two ways to install `DiffEqJump.jl`. First, users may install the meta
`DifferentialEquations.jl` package, which installs and wraps `OrdinaryDiffEq.jl`
for solving ODEs, `StochasticDiffEq.jl` for solving SDEs, and `DiffEqJump.jl`,
along with a number of other useful packages for solving models involving ODEs,
SDEs and/or jump process. This single install will provide the user with all of
the facilities for developing and solving Jump problems.

To install the `DifferentialEquations.jl` package, refer to the following link
for complete [installation
details](https://docs.sciml.ai/dev/modules/DiffEqDocs/).

If the user wishes to separately install the `DiffEqJump.jl` library, which is a
lighter dependency than `DifferentialEquations.jl`, then the following code will
install `DiffEqJump.jl` using the Julia package manager:
```julia
using Pkg
Pkg.add("DiffEqJump")
```

## Contributing
- Please refer to the
  [SciML ColPrac: Contributor's Guide on Collaborative Practices for Community Packages](https://github.com/SciML/ColPrac/blob/master/README.md)
  for guidance on PRs, issues, and other matters relating to contributing to SciML.
- There are a few community forums:
    - the #diffeq-bridged and #sciml-bridged channels on the [Julia Slack](https://julialang.org/slack/)
    - [JuliaDiffEq](https://gitter.im/JuliaDiffEq/Lobby) on Gitter
    - the [Julia Discourse forums](https://discourse.julialang.org)
See also the [SciML Community page](https://sciml.ai/community/).