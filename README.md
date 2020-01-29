# Automatic Scientific Annotation
This repository contains the automatically annotated citations for the [SciSummNet dataset](https://cs.stanford.edu/~myasu/projects/scisumm_net/). The annotation method uses the pivot-based classification model presented in the paper [link to the paper](link).

## Repository Organization
The repository is organized as follow:
- The `pivot_words` directory contains the pivot words both for the referring and the cited sentences extracted from the test set using [link](https://arxiv.org/abs/1909.12335).
- The `annotations` folder contains the output of the automatic annotation described in the paper [link to the paper](link). For each paper the annotations are proposed in a `.tsv` where each line is formatted as: `citation_id  citation_type`.

