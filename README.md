# DocumenterTools

| **Build Status**                                                                                |
|:-----------------------------------------------------------------------------------------------:|
| [![][travis-img]][travis-url] [![][appveyor-img]][appveyor-url] [![][codecov-img]][codecov-url] |

This package enables the Markdown / MkDocs backend of [`Documenter.jl`][documenter].

## Installation

The package is currently unregistered and must be added via URL in the package manager.
From the Julia REPL, type `]` to enter the Pkg REPL mode and run

```
pkg> add https://github.com/JuliaDocs/DocumenterMarkdown.jl.git
```

## Usage

To enable the backend import the package in `make.jl` and then just pass `format = :markdown`
to `makedocs`:

```julia
using Documenter
using DocumenterMarkdown
makedocs(format = :markdown, ...)
```

[documenter]: https://github.com/JuliaDocs/Documenter.jl
[documenter-docs]: https://juliadocs.github.io/Documenter.jl/stable/

[docs-stable-img]: https://img.shields.io/badge/docs-stable-blue.svg
[docs-stable-url]: https://juliadocs.github.io/DocumenterMarkdown.jl/stable

[travis-img]: https://travis-ci.org/JuliaDocs/DocumenterMarkdown.jl.svg?branch=master
[travis-url]: https://travis-ci.org/JuliaDocs/DocumenterMarkdown.jl

[appveyor-img]: https://ci.appveyor.com/api/projects/status/mi763gn92pb6rxly?svg=true
[appveyor-url]: https://ci.appveyor.com/project/JuliaDocs/documentermarkdown-jl

[codecov-img]: https://codecov.io/gh/JuliaDocs/DocumenterMarkdown.jl/branch/master/graph/badge.svg
[codecov-url]: https://codecov.io/gh/JuliaDocs/DocumenterMarkdown.jl