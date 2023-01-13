# Isabelle Tools Collection
[![Build Status](https://ci.isabelle.systems/jenkins/buildStatus/icon?job=isabelle-notify&subject=Isabelle%2Fdevel%3A%20%24%7BstartTime%7D%20ago)](https://ci.isabelle.systems/jenkins/job/isabelle-notify/)

This is a collection of maintained [Isabelle](https://isabelle.in.tum.de) add-on tools.
Most are Isabelle/Scala components that are either very niche, too experimental,
or not stable enough, to have made it into the distribution (yet).

Each tool resides in its own repository.
This page merely gives an overview,
and provides tooling to trigger ci pipelines on Isabelle changes.
All tools have a status badge indicating whether they work with the latest Isabelle development version.

## Tool list
### [Isabelle Linter](https://github.com/isabelle-prover/isabelle-linter) ![status](https://github.com/isabelle-prover/isabelle-linter/actions/workflows/build.yml/badge.svg)
Isar linter for Isabelle/HOL.
### [Isabelle Context Build](https://github.com/isabelle-prover/isabelle-context-build) ![status](https://github.com/isabelle-prover/isabelle-context-build/actions/workflows/build.yml/badge.svg)
Contextualized build tool with slurm cluster build.

## Adding a tool to the collection
If you maintain an Isabelle tool, you can add it to the collection as follows:
1. Add code to [ci_notify](src/ci_notify.scala) (inside dispatch method, where commented) to trigger your build on Isabelle changes
2. Add your tool with link and build badge to the list