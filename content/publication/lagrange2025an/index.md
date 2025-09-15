---
title: An Efficient Search-and-Score Algorithm for Ancestral Graphs using Multivariate Information Scores for Complex Non-linear and Categorical Data
authors:
- admin
- Hervé Isambert
author_notes:
date: '2025-05-01'
publishDate: '2025-06-24T16:41:15.035541Z'
reading_time: false
share: false
publication_types:
- paper-conference
publication: '*Forty-second International Conference on Machine Learning (ICML 2025)*'
abstract: 
    We propose a greedy search-and-score algorithm for ancestral graphs, which include directed as well as bidirected edges, originating from unobserved latent variables. The normalized likelihood score of ancestral graphs is estimated in terms of multivariate information over relevant "*ac*-connected subsets" of vertices, _**C**_, that are connected through collider paths confined to the ancestor set of _**C**_. For computational efficiency, the proposed two-step algorithm relies on local information scores limited to the close surrounding vertices of each node (step 1) and edge (step 2). This computational strategy, although restricted to information contributions from *ac*-connected subsets containing up to two-collider paths, is shown to outperform state-of-the-art causal discovery methods on challenging benchmark datasets.

tags:
- Information Theory
- Machine Learning
- Search-and-Score
- Structure Learning
- Latent Variable
- Causal Discovery
- Methodology
- Multivariate Information
links:
- name: URL
  url: https://openreview.net/forum?id=RfqTvlo9XQ
url_code: 'https://github.com/miicTeam/miicsearchscore'
url_poster: 'poster.pdf'
---
