Information Set Decoding (ISD) – Python Implementation

This repository contains a clean and modular implementation of the Information Set Decoding (ISD) algorithm over GF(2).
It includes both randomized ISD and systematic (combinatorial) ISD, along with utilities for:

Matrix inversion over GF(2)

Encoding messages

Searching for low-weight error vectors

Running experiments with random linear codes

This is a small educational project demonstrating how ISD works on small parameters.

Features
✔ GF(2) Linear Algebra

Custom implementation of matrix inversion in GF(2)

Bitwise row operations

Full support for binary linear codes

✔ Message Encoding

encode_message(x, G) computes 
c=xGmod  2
c=xGmod2

✔ Randomized ISD

Samples random information sets

Checks invertibility of selected columns

Recovers t-error patterns when possible

Tracks statistics:

number of trials

number of non-invertible sets

success flag

recovered information set

✔ Systematic ISD (Combinatorial)

Brute-force enumeration of all size-k subsets

Deterministic but slower

Useful for correctness testing

✔ Example Experiments

Works on a fixed (8,16) linear code


Demonstrates decoding of an error of weight 2

Includes random test cases with full-rank generator matrices
