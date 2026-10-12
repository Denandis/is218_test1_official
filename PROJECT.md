# IS218 Test 1 — Calculator

**Name:** Nandish Desai

## Purpose

A small Python calculator package that provides addition and subtraction,
tested with pytest. Another developer can clone it, install the dependencies,
and run the test suite to confirm it works.

## Setup and test commands

Create and activate the environment, then install the dependencies:

    python3 -m venv .venv
    source .venv/bin/activate
    python -m pip install -r requirements.txt

Run the student test suite:

    python -m pytest

Run the student tests together with the supplied acceptance checks:

    python -m pytest tests checks -v

## Issues

Issue creation is restricted on this fork, so issues could not be opened.
The work was completed in the matching branches and merged into `main`:

- Setup (branch `setup`)
- Addition (branch `addition`)
- Subtraction (branch `subtraction`)
- Delivery (branch `delivery`)

## One test explained

In `tests/operations/test_add.py`, the test `test_add` calls `add(2, 3)`.
The expected result is `5`, because adding 2 and 3 gives 5. The assertion
`assert result == 5` fails if the function returns anything else, which
confirms the addition function computes from its arguments.

## Why .venv is ignored

The `.venv` directory is ignored and not committed because it is large,
machine-specific, and can be recreated on any computer. The
`requirements.txt` file is committed so that anyone who clones this project
can rebuild the same environment by running
`python -m pip install -r requirements.txt`.
