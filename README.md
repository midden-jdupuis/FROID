# FROID_NS

FROID is a self-hosting framework for addressable intent. It lets a project define semantic contracts as immutable FOLIOs, then realize those contracts into code, documentation, tests, prompts, or other artifacts.

This repository contains the FROID namespace specification and early tooling.

## Why

FROID began as infrastructure for building software with AI assistance while preserving human intent. Generated code can work while drifting away from the specification that produced it. FROID gives intent a durable, addressable layer above implementation.

## Core ideas

- NODE_ID: stable structured identifier
- FOLIO: committed semantic record
- FLIO_REF: manifest that establishes a FOLIO
- Supersession: change by replacement, not mutation
- Realization: output artifact produced from a selected FOLIO stack
- Superego: realization policy and constraints

## Repository layout

- `namespace/` — self-hosted FROID namespace
- `tools/` — validators, prompt compilers, and utility scripts
- `README.md` — public overview
- `CLAUDE.md` / `AGENTS.md` — minimal agent instructions

## Status

Experimental. The namespace is being prepared for v1.0 FOLIO locking and public tooling.