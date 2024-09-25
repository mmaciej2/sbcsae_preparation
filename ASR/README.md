### Annotations for ASR Evaluation

- `aligned_for_asr.stm` (preferred) – STM file for the realignments targeting ASR evaluation, with excessive bounding silence trimmed in a conservative manner to ensure all words lie within the boundaries
- `aligned_for_diar.stm` (non-preferred) – STM file for the realignments targeting diarization evaluation, with segements more closely tracking the true voice activity, at the cost of some words potentially having been trimmed
- `original.stm` (non-preferred) – STM file for the original segmentation of the corpus
