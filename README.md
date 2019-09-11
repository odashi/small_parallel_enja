small_parallel_enja: 50k En/Ja Parallel Corpus for Testing SMT Methods
======================================================================

This directory includes a small parallel corpus for English-Japanese
translation task. These data are extracted from
[TANAKA Corpus](http://www.edrdg.org/wiki/index.php/Tanaka_Corpus)
by filtering sentence length 4 to 16 words.

English sentences are tokenized using
[Stanford Tokenizer](http://nlp.stanford.edu/software/tokenizer.html)
and lowercased.
Japanese sentences are tokenized using [KyTea](http://www.phontron.com/kytea/).

All texts are encoded in UTF-8. Sentence separator is `'\n'` and word separator
is `' '`.

**Attention**: some English words have different tokenization results from Stanford Tokenizer,
e.g., "don't" -> "don" "'t", which may came from preprocessing errors.
Please take care of using this dataset in token-level evaluation.

Corpus Statistics
-----------------

| File           | #sentences |  #words | #vocabulary |
|:---------------|-----------:|--------:|------------:|
| train.en       |     50,000 | 391,047 |       6,634 |
| - train.en.000 |     10,000 |  78,049 |       3,447 |
| - train.en.001 |     10,000 |  78,223 |       3,418 |
| - train.en.002 |     10,000 |  78,427 |       3,430 |
| - train.en.003 |     10,000 |  78,118 |       3,402 |
| - train.en.004 |     10,000 |  78,230 |       3,405 |
| train.ja       |     50,000 | 565,618 |       8,774 |
| - train.ja.000 |     10,000 | 113,209 |       4,181 |
| - train.ja.001 |     10,000 | 112,852 |       4,102 |
| - train.ja.002 |     10,000 | 113,044 |       4,105 |
| - train.ja.003 |     10,000 | 113,346 |       4,183 |
| - train.ja.004 |     10,000 | 113,167 |       4,174 |
| dev.en         |        500 |   3,931 |         816 |
| dev.ja         |        500 |   5,668 |         894 |
| test.en        |        500 |   3,998 |         839 |
| test.ja        |        500 |   5,635 |         884 |
