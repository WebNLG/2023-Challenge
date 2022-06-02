# Data

We provide rough training data automatically translated from the original 2020 English set into the 3 target languages via a multilingual [NMT system](https://github.com/bzhangGo/zero/tree/master/docs/multilingual_laln_lalt). We also provide dev sets that have been manually translated into each target language by human translators.

The [benchmark reader](../utils) can be used to load and parse these datasets.

Language codes are as follows:
* Breton - `br`
* Welsh - `cy`
* Irish - `ga`
* Maltese - `mt`

The Breton development set (`br_dev.xml`) contains 1399 entries from the WebNLG 2020 English dev set that have each had one lexicalisation manually translated to Breton. These entries were randomly sampled while making sure to cover lexicalisations from all triple set size groups.

The development sets for the remaining languages each contain 1665 manually translated entries from the WebNLG 2020 English dev set (entries 485 and 808 have been excluded).
