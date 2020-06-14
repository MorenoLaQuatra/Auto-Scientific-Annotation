# Automatic Scientific Annotation
This repository contains the automatically annotated citations for the [ScisummNet dataset](https://cs.stanford.edu/~myasu/projects/scisumm_net/) using the classifier trained on the annotated collection [scisumm-corpus](https://github.com/WING-NUS/scisumm-corpus). The annotation method uses the pivot-based classification model presented in this [paper](https://doi.org/10.1007/s11192-020-03532-3).

## Repository Organization
The repository is organized as follow:
- The [pivot_words](pivot_words) directory contains the pivot words both for the citing and the cited sentences extracted from the scisumm-corpus training set using the method described [here](https://arxiv.org/abs/1909.12335). Implementation available in this [repository](https://github.com/FranxYao/pivot_analysis).
- The [annotations](annotations) folder contains the output of the automatic annotation described in the paper [link to the paper](link). For each paper the annotations are proposed in a `.tsv` where each line is formatted as: `citation_id  citation_type`.
- The [hyp_facet_summaries](hyp_facet_summaries) directory contains one subfolder for each paper in the test set. Each subfolder contains the proposed facet summaries by different regression models.
- The [ref_facet_summaries](ref_facet_summaries) directory contains the gold facet summaries for each pair paper - citation facet.
- The [reproducibility](reproducibility) directory contains the train/test key split to reproduce the results of the paper.


## Annotation examples

|    Facet    |  Type  |                                                                                                                                                                                                                        Text                                                                                                                                                                                                                        |
|:-----------:|:------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|    Method   | Citing | We used the base feature model defined in (Nivre et al, 2006) for all the languages but Arabic, Chinese, Czech, and Turkish.                                                                                                                                                                                                                                                                                                                       |
|             |  Cited | Features of the type DEPREL have a special status in that they are extracted during parsing from the partially built dependency graph and may therefore contain errors, whereas all the other features have gold standard values during both training and parsing.2 Based on previous research, we defined a base model to be used as a starting point for languagespecific feature selection.                                                     |
|   Results   | Citing | These parameters are identical to Nivre et al (2006b) to enable a,comparison of the scores. We evaluated the feature candidates on a,development set using the labeled and unlabeled attachment scores (LAS,and UAS) that we computed with the eval.pl script from CoNLL-X.                                                                                                                                                                        |
|             |  Cited | This is noticeable for German (Brants et al., 2002) and Portuguese,(Afonso et al., 2002), which still have high overall accuracy thanks to,very high attachment scores, but much more conspicuous for Czech,(B¨ohmov´a et al., 2003), Dutch (van der Beek et al., 2002) and Slovene,(Dˇzeroski et al., 2006), where root precision drops more drastically to,about 69\%, 71\% and 41\%, respectively, and root recall is also affected,negatively. |
| Implication | Citing | We split German compound words (mostly nouns), based on the frequency of the words in the potential decompositions (Koehn and Knight, 2003a).                                                                                                                                                                                                                                                                                                      |
|             |  Cited | One reason for this is that the system recovers more easily from words that are split too much than from words that are not split up sufficiently.                                                                                                                                                                                                                                                                                                 |
|     Aim     | Citing | the possible part(s)-of-speech of unknown words (Mikheev,1997).                                                                                                                                                                                                                                                                                                                                                                                    |
|             |  Cited | In this paper we present a technique for fully automatic acquisition of rules that guess possible part-of-speech tags for unknown words using their starting and ending segments.                                                                                                                                                                                                                                                                  |

## Citation

If you use this material in your research work please let us know citing our [paper](https://doi.org/10.1007/s11192-020-03532-3) as follows:

La Quatra, M., Cagliero, L. & Baralis, E. Exploiting pivot words to classify and summarize discourse facets of scientific papers. Scientometrics (2020). https://doi.org/10.1007/s11192-020-03532-3




