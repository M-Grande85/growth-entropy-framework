# Growth–Entropy Framework

This repository provides a reference implementation of a growth–entropy diagnostic framework for nonlinear dynamical systems.

## Core idea

Irreversible growth is defined as the accumulation of structural constraint that reduces the set of dynamically accessible future macrostates of a system. Growth is not identified with time evolution, energy increase, or entropy production alone. Instead, growth corresponds to the contraction of accessible future outcomes under admissible perturbations.

## Operational definition

For a system in state X(t), with perturbation scale ε and forecast horizon τ, define Ωε(t,τ) as the set of distinct macroscopic outcomes reachable under perturbations ≤ ε. The effective volume of this set, V(t,τ), can be estimated empirically using ensemble divergence or outcome clustering.

Accumulated growth is defined as:

g(t) = − ln V(t,τ)

Growth rate therefore corresponds to the relative rate at which accessible future states collapse.

## Entropy constraint

Irreversible growth incurs entropy production and is constrained by entropy export capacity γ according to:

dS/dt = α (dg/dt)² − γ S

Rapid contraction of accessible futures is entropy-expensive and bounded by available entropy export. When entropy export capacity collapses (e.g., near horizons), irreversible growth stalls even if local dynamics continue.

## What this repository contains

This repository is intended as a minimal, model-agnostic reference implementation. It includes:

- Formal definitions of growth and accessible future states
- Toy examples demonstrating state-space contraction
- Diagnostic methods that operate without modifying system dynamics
- Illustrations of entropy-limited regime commitment

## What this repository is not

- It is not a numerical weather prediction model
- It is not a new dynamical law or force
- It does not modify governing equations
- It does not claim extended predictability beyond chaos limits

## Status

This repository accompanies a theoretical framework developed for publication and is intended to support inspection, testing, and extension of the core ideas.
