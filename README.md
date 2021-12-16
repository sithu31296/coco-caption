Microsoft COCO Caption Evaluation
===================

Evaluation codes for MS COCO caption generation.

This is a new fork from [ruotianluo/coco-caption](https://github.com/ruotianluo/coco-caption) which fixes the following:

* METEOR evaluation error
* SPICE evaluation error (Caching error in Windows)
* Windows Installation setup

Other details can be seen in the forked repo.


## Requirements

* java 1.8.0
* python 3
* gensim
* pyemd

> For Windows, download java from [here](https://www.java.com/en/download/manual.jsp).

## Installation

For Linux:

```bash
$ ./get_stanford_models.sh
$ ./get_google_word2vec_model.sh
```

For Windows:

* Download Stanford CoreNLP model from [here](http://nlp.stanford.edu/software/stanford-corenlp-full-2015-12-09.zip).
* Extract the zip file.
* Copy `stanford-corenlp-3.6.0.jar` and `stanford-corenlp-3.6.0-models.jar` to `pycocoevalcap/spice/lib`.
* Download Google News negatie 300 word2vec model from [here](https://s3.amazonaws.com/dl4j-distribution/GoogleNews-vectors-negative300.bin.gz).
* Extract the zip file.
* Copy `GoogleNews-vectors-negative300.bin` to `pycocoevalcap/wmd/data`.