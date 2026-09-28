# Tensor-Train-Compressed-Separable-PINNs

This repository provides supporting code for the ablation studies presented in the arXiv paper

Tensor-Train Compressed Separable PINNs: A Curvature-Aware Optimization Framework for Parametric PDEs in High Dimensions.

# Overview

The paper develops a curvature-aware optimization framework for physics-informed neural networks (PINNs) applied to high-dimensional and parametric PDEs. The main idea is to combine coordinate-separable neural architectures, in particular tensor-train (TT) representations, with a structured Gauss--Newton method.

By exploiting separability of both the neural representation and the differential operator, the residual Jacobian admits a structured factorization. This allows the Gauss--Newton step to be computed in a much smaller compressed residual space, avoiding explicit construction of the full residual Jacobian and the exponentially large tensor-product collocation grid.

The numerical studies investigate, among other aspects,

- the effect of tensor compression and tensor-train ranks;

- the effective dimension of the compressed Gauss--Newton system;

- optimization with compressed Gauss--Newton compared with first-order training;

- high-dimensional Poisson problems; and

- high-dimensional parametric Darcy problems with different levels of parametric complexity.

The code in this repository contains focused implementations and scripts supporting these numerical ablation studies.
