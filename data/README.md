# Data

We provide versions of the original 2020 English development set which have been manually translated into each of the 4 target language by human translators.

Language codes are as follows:
* Breton - `br`
* Welsh - `cy`
* Irish - `ga`
* Maltese - `mt`

We also provide optional silver training data that has been automatically translated into the 4 target languages from the original English set via a multilingual [NMT system](https://github.com/bzhangGo/zero/tree/master/docs/multilingual_laln_lalt).

The [benchmark reader](../utils) can be used to load and parse these datasets.

| Language     | No. Dev Items | No. Train Items |
|--------------|---------------|-----------------|
| Breton (br)  | 1,399         | 13,211          |
| Welsh (cy)   | 1,665         | 13,211          |
| Irish (ga)   | 1,665         | 13,211          |
| Maltese (mt) | 1,665         | 13,211          |

Note:
* Due to translation constraints, the Breton development set (`br_dev.xml`) only contains 1399 entries from the WebNLG 2020 English dev set. These entries were randomly sampled while making sure to cover lexicalisations from all triple set size groups.
* All other languages contain manual translations of all but 2 entries from the WebNLG 2020 English dev set (entries 485 and 808 have been excluded).
