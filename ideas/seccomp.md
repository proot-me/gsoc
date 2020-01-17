# Implementing libseccomp

_libseccomp provides an easy to use, platform independent, interface to the Linux Kernel's syscall filtering mechanism_

## Description

There is currently a [major flaw](https://github.com/proot-me/proot/issues/106) with PRoot's seccomp implementation resulting in a segmentation fault on Linux kernels newer than the 4.8 version. Despite [patches](https://github.com/proot-me/proot/pull/130) to address this, some of the core tests from the testsuite are still failing on modern kernels. Instead of maintaining the legacy seccomp code, we would like to see [libseccomp implemented](https://github.com/proot-me/proot/issues/195). Below is a brief excerpt of the benefits this solution would provide:

> We (libseccomp) will take care of cBPF creation, ABI issues,
and any syscall changes when a new kernel is released. Maintaining a custom
filter throughout all of that can be challenging.

This would also help with portability since libseccomp supports [several different architectures](https://github.com/seccomp/libseccomp#supported-architectures).

## Outcomes

The current testsuite should pass on recent Linux kernels with no failures, on all of the arches that PRoot supports.

## Requirements

c, git, linux, ptrace, syscalls, seccomp

## Mentor(s)

Lucas Ramage

## Difficulty

Hard
