---
year: 2020
---

# PRoot / CARE and Intel SGX

_Utilize PRoot / CARE in an Intel SGX enclave_

## Description

There are quite a few solutions that enable running docker images in an SGX enclave (Scone, Graphene-ng, Fortanix, etc.), but they are all either proprietary or hard to manipulate. It'd be nice to be able to use the combo PRoot/care to package a runtime for later re-execution within Intel SGX.

## Outcomes

Proof of concept implementation for running container in an enclave.

## Requirements

c, git, ptrace, sgx, encryption

## Mentor(s)

Lucas Ramage, Jonathan Passerat-Palmbach

## Difficulty

Hard
