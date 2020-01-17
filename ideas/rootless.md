# Unprivileged containers

_Running unprivileged containers via PRoot_

## Description

OCI containers can be built and/or downloaded using [img](https://github.com/genuinetools/img), 
and then run as any user via PRoot. There is already a proof of concept in progress, (See: https://github.com/proot-me/proot/pull/204), however, it is very rough, and there are several open bugs that still need to be patched before this can be merged upstream. We will also need some tests built out for the testsuite in order to ensure there are no regressions.

## Outcomes

A solution for running unprivileged OCI-compatible containers via PRoot.

## Requirements

c, git, go, linux, containers

## Mentor(s)

Lucas Ramage

## Difficulty

Medium
