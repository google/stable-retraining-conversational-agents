# Random and Systematic Noisy Data for Stable Re-training of Conversational Agents

This repository contains the synthetic data for the paper:

*   Reducing Model Churn: Stable Re-training of Conversational Agents

The data is derived from the following datasets:

*   [Semantic Parsing for Task Oriented Dialog using Hierarchical
    Representations](https://research.fb.com/publications/semantic-parsing-for-task-oriented-dialog-using-hierarchical-representations/)
*   [Low-Resource Domain Adaptation for Compositional Task-Oriented Semantic Parsing](https://fb.me/TOPv2Dataset)    
*   [MTOP: A Comprehensive Multilingual Task-Oriented Semantic Parsing Benchmark](https://fb.me/mtop_dataset)
*   [Snips Voice Platform: an embedded Spoken Language Understanding system for private-by-design voice interfaces](https://github.com/sonos/nlu-benchmark)

## Data

The generated synthetic data is present in the following directories (corresponding respectively to the above links):

    top_data/
    
    topv2_data/
    
    mtop_data/
    
    snips_data/
    
Each dataset directory has two subdirectories:

    swap_top/
    
    distant_top/

These subdirectories contain the random and systematic noisy datasets from Section 6.

Each dataset will have a train.tsv file with columns for "query" and "label."

The dev and test sets are the same as the original papers and are thus not included here.

The distant_top directories have an additional file named distant_labeled_train.tsv, which corresponds to the heldout 10\% of the training data that was labeled by a model.
