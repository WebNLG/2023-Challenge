# Baselines

Included are system outputs for a range of baselines.

* `amazon_en2<tgt>_test.<tgt>` - Amazon rdf2text model fed into NMT system.
* `forge2017_en2<tgt>_test.<tgt>` - FORGE2017 rdf2text baseline fed into NMT system.
* `forge2020_en2<tgt>_test.<tgt>` - FORGE2020 rdf2text baseline fed into NMT system.

Each baseline uses an RDF-to-Text system from the WebNLG 2020 Challenge to generate an English lexicalisation which is fed into the [Zero neural machine translation sytem](https://arxiv.org/abs/2004.11867) to get a translation in  the target language. We use the 24-layer with back-translation version of Zero, available [here](https://github.com/bzhangGo/zero/tree/master/docs/multilingual_laln_lalt).

### Results for Breton

|           | BLEU  | BLEU_nltk | METEOR | chrF++ | TER  |
|-----------|-------|-----------|--------|--------|------|
| Amazon    | 11.82 | 0.11      | 0.28   | 0.33   | 0.77 |
| FORGE2020 | 9.23  | 0.08      | 0.23   | 0.3    | 0.76 |
| FORGE2017 | 8.79  | 0.08      | 0.22   | 0.29   | 0.77 | 


