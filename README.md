# Supplementary materials for 'Signal smoothing and syntactic choices: A critical reflection on the UID hypothesis'

This repository contains materials accompanying the Open Mind submission "Signal smoothing and syntactic choices: A critical reflection on the UID hypothesis". 



## Components

1) C-SALT.tsv
2) C-SALT_uid_analysed.tsv
3) uids_gpt3.py
4) Table X
5) Additional plots

---

### C-SALT.tsv

The Corpus of Syntactic ALTernations (C-SALT) is attached as a separate file. This corpus includes nine syntactic phenomena considered alternations in the linguistic literature. The items are sourced from various licensed materials (see LICENSE.md for details). The corpus has been pre-processed for parsing, involving the removal of special characters and final punctuation, which is not expected to have a negative impact on the results. Annotations within the corpus are mostly self-explanatory.

Critically, each construction in the corpus has two types:

Occurrences of the phenomenon, along with their hypothetical baseline counterparts.
Reversed occurrences where real baseline examples are transformed to include the phenomenon.
For example, a real occurring cataphora sentence is "When she begins a new work, Freeman first sketches out an idea" while the constructed hypothetical counterpart is "When Freeman begins a new work, she first sketches out an idea". Similarly, a real occurrence of a sentence in canonical word order might be "And because Ben was the stronger and the faster, he always won" while the hypothetical counterpart containing a cataphora is "And because he was the stronger and the faster, Ben always won".

The naturalness of the constructed items was evaluated by a native English speaker. Items of reduced naturalness were still included as their inclusion favours the UID hypothesis, if anything. 

However, please note that there is a selection bias in the corpus. From the paper: "Difficult-to-construct counterparts in either direction were skipped, such as cases where constructing a baseline counterpart for extrapositions was challenging or when an extraposition was not a viable option for a sentence in canonical word order. This practical approach ensures a focus on meaningful alternations rather than including imbalanced ones. Arguably, including more of imbalanced alternatives might have tipped the scale slightly in favor of the UID hypothesis, but we would expect the effect on the Low-IC theory be even larger."



### C-SALT_uid_analysed.tsv

This file contains the analysis of C-SALT using GPT-3.5 (text-davinci-003, as per https://platform.openai.com/docs/models/gpt-3-5) to collect surprisal values. These values were used to test the different frameworks discussed in the Open Mind paper. Please be aware that the number of tokens is according to GPT-3.5, which is typically 'no_words - 1', although there may be cases where it differs slightly. However, this difference should not distort the analyses.
Results from GPT-2 were also included and come out similarly. 



### uids_gpt3.py

This is the rapid development script used to do the analyses for the items. Note that surprisal values slightly fluctuate between executions. 



### Table X

In response to a reviewer's suggestion, a table summarising the literature and different papers' perspectives on the UID hypothesis has been included, as part of this readme. It aims to provide an overview of what various papers have to say about UID. While creating a fair and comprehensive overview is challenging, this table can be adjusted if needed, as it is part of this repository and not a static element in a published paper.

| Category        | Literature           | 
| ------------- |:-------------:| 
| Positive results (in supoprt of UID)      | Paper A1 <br /> Paper A2| 
| Mixed results      | Paper B      | 
| Inconclusive results | Paper C      | 
| Negative results | Paper D      | 



### Additional plots

The plot in the paper is rather dense, so this repository includes additional plots for further clarification. 

This is Figure 3 from the paper with colour coding (taken from https://davidmathlogic.com/colorblind): 

![fig3colour](https://github.com/arizus/uid/blob/main/alternationsresults3_colour.png?raw=true)

Here, constructions highlighted for which the data comes from exclusively spoken corpora: 

![fig3spoken](https://github.com/arizus/uid/blob/main/alternationsresults3_spoken.png?raw=true)

In the following plot, surprisal values were extracted using GPT-2. While the F1-Scores exhibit slight variation, the UID variants continue to face challenges and are surpassed by the Low-IC hypothesis:

![fig3spoken](https://github.com/arizus/uid/blob/main/alternationsresults_gpt2.png?raw=true)

---



## License

The materials in this repository are licensed under [license name]. Please see the LICENSE.md file for more information. 



## Contact

[email]

