# PageRank: A Technical Case Study

A mathematical analysis of Google's PageRank algorithm and the linear-algebraic
ideas underlying ranking on directed networks.

## Overview

PageRank assigns importance scores to webpages using the structure of incoming
and outgoing links. This case study develops the algorithm from a stochastic
matrix representation of the web and explains how a stationary distribution can
be used as a ranking vector.

The report focuses on both the mathematical formulation and the practical issues
that arise when the link network is not directly suitable for a Markov-chain
model.

## Topics Covered

- Directed graphs and hyperlink matrices
- Column-stochastic transition matrices
- Random-surfer interpretation
- Stationary distributions and dominant eigenvectors
- Dangling nodes and disconnected components
- Damping and the Google matrix
- Convergence and interpretation of PageRank scores

## Repository Contents

- `PageRank_Technical_Report.pdf` - complete mathematical case study.

## Mathematical Formulation

Given a suitable transition matrix \(P\), PageRank seeks a probability vector
\(r\) satisfying

\[
r = Pr.
\]

With damping parameter \(\alpha\) and \(n\) pages, the Google matrix can be
written as

\[
G = \alpha P + (1-\alpha)\frac{1}{n}\mathbf{1}\mathbf{1}^{T}.
\]

The PageRank vector is then the stationary distribution of \(G\).

## Key Skills Demonstrated

Linear algebra, Markov chains, eigenvalue methods, network analysis,
mathematical exposition, and technical writing.

