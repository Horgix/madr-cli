# Markdown Architectural Decision Records - Command Line Interface

`madr-cli` is a small command line interface to create and manage ADRs
(Architectural Decision Records) using [_madr_ (Markdown
ADR)](https://adr.github.io/madr/) as format.

## Objectives

`madr-cli` aims for:

- Simplicity of usage. Everything should make sense out of the box
- Configurability of madr optionnal sections
- Portability

Of course, `madr-cli` uses madr to record its own decisions 🙂

## How is it different from `adr-tools` ?

You might already know [`adr-tools`](https://github.com/npryce/adr-tools) that
fits a similar need. However:

- `adr-tools` is written in pure shell and thus depends on some external tools
  such as grep, sed, awk, etc., making it environment-dependant and not that
  much portable.
- At time of writing, `adr-tools` is unmaintained for 3+ years
- At time of writing, the CI of `adr-tools` is reporting to fail
