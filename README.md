# Prague Manifesto – Multilingual Parsed Corpus (CoNLL-U)

## Overview

This repository contains parsed linguistic data derived from the **Prague Manifesto** (source: [https://lingvo.org/prago](https://lingvo.org/prago)).
The texts are provided in **20 different languages** (Catalan, Croatian, Danish, Dutch, English, Finnish, French, German, Greek, Hungarian, Italian, Japanese, Lithanian, Polish, Portuguese, Romanian, Russian, Slovenian, Spanish, and Swedish) and have been automatically annotated using **Universal Dependencies (UD)** standards.

All parsed outputs are stored in **CoNLL-U format**, making the dataset suitable for computational linguistics, corpus linguistics, and NLP research.

---

## Data Description

* **Source text**: Prague Manifesto
* **Number of languages**: 20
* **Annotation scheme**: Universal Dependencies
* **File format**: CoNLL-U (`.conllu`)

Each file corresponds to one language version of the manifesto and contains:

* Tokenization
* Lemmatization
* Part-of-speech tagging
* Morphological features
* Dependency relations

---

## Parsing Tools and Models

### Hungarian

* **Library**: HuSpaCy
* **Model**: `hu_core_news_lg`

### All Other Languages

* **Library**: SpaCy
* **Models**: Official SpaCy language models available for each respective language at the time of parsing

---

## Parsing Script

The parsing was performed using the following Python script:

* **Script name**: `textAnalysis_moya.py`

This script:

1. Loads the appropriate SpaCy or HuSpaCy language model,
2. Processes the raw text of the Prague Manifesto,
3. Outputs syntactic and morphological annotations in CoNLL-U format.

---

## Folder Contents

* `*.conllu` files – Parsed versions of the Prague Manifesto for each language

---

## Intended Use

This dataset is intended for:

* Comparative syntactic analysis
* Cross-linguistic studies
* NLP model evaluation
* Educational purposes in dependency grammar and corpus annotation

---

## Notes and Limitations

* The annotations are **automatically generated** and may contain errors.
* Model quality and annotation accuracy vary across languages, depending on the maturity of the underlying SpaCy models.
* The dataset reflects the state of the models at the time of parsing and has not been manually corrected.

---

## License and Source Acknowledgment

* Original text: Prague Manifesto ([https://lingvo.org/prago](https://lingvo.org/prago))
* Users are responsible for ensuring compliance with the original text’s licensing terms when redistributing or publishing derived data.

---

