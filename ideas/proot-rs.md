---
year: 2020
---

# Rust Port

_Rust implementation of PRoot, a ptrace-based sandbox_

## Description

There is already a proof of concept in progress, (See: https://github.com/proot-me/proot-rs). However, this implementation is very basic and only runs on a single architecture. Work is still needed to complete a functioning prototype, as outlined here, <https://github.com/proot-me/proot-rs/issues/1>:

> Remaining steps for the bare minimum (single-tracee, no glue, no extensions, no ptrace-translation, no unix-socket translation, no qemu, -r/-R, -w and -b cli options only, no seccomp, and x86-64 with 64bits programs only)

## Outcomes

Fully functional, albeit minimal, PRoot implementation written in Rust.

## Requirements

git, ptrace, rust

## Mentor(s)

Lucas Ramage

## Difficulty

Medium
