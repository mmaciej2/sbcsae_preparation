# Data Preparation for the Santa Barbara Corpus of Spoken American English

This respository contains the supplemental information to accompany the paper "[Evaluating the Santa Barbara Corpus: Challenges of the Breadth of Conversational Spoken Language](https://www.isca-archive.org/interspeech_2024/maciejewski24_interspeech.html)".
This includes the final annotation files used for evaluation, links to the code used to prepare the data, and additional statistics on the corpus.

If you use our work, please cite the paper:
```
@inproceedings{maciejewski24_interspeech,
  author={Matthew Maciejewski and Dominik Klement and Ruizhe Huang and Matthew Wiesner and Sanjeev Khudanpur},
  title={Evaluating the {Santa Barbara} Corpus: Challenges of the Breadth of Conversational Spoken Language},
  year=2024,
  booktitle={Proc. Interspeech 2024}
}
```

## Annotations for Evaluation

The most comprehensive set of annotations can be found in the [Lhotse](https://github.com/mmaciej2/lhotse/tree/sbcsae) recipe, which also includes code to download the corpus.
However, if you would like to merely download the basic annotation files for use with your own systems without using Lhotse, these files can be found in the "ASR" and "Diarization" subdirectories of this respository.

## Preparation Scripts

The code that was used to prepare the data is contained in three repositories:

- [Lhotse Recipe](https://github.com/mmaciej2/lhotse/tree/sbcsae) - The Lhotse recipe contains the bulk of the processing, normalization, and correction required to prepare the annotations and metadata for automatic processing. It also contains code to download the corpus.
- [Anonymization Detection](https://github.com/mmaciej2/sbcsae_anon_detection) - This repository contains the code used to detect the regions of the audio that had been low-pass filtered to remove personally identifiable information from the speech.
-  Alignment for VAD - This repository contains the code used to align the transcripts to re-segment single-speaker regions for better voice activity detection (VAD) boundaries.

## Corpus Statistics

TODO
