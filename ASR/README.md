### Annotations for ASR Evaluation

- aligned_for_asr.stm (preferred): Re-aligned segments containing a lot of silence only to make sure all the spoken words are within the re-aligned boundaries).
- aligned_for_diar.stm (non-preferred): The boundaries are thighter, some words may be cut short.
- original.stm (depends): Original not aligned segments.

##### Suggestions
If you do not care about the segmentation, the choice of the stm files does not matter; however, aligned stm files contain manual dataset fixes, such as added redactions or marked words that are not audible (ToDo: Add description of the manual data corrections).
If you want to cut audio based on the ground truth segmentation, we strongly advice to use `aligned_for_asr.stm`.
If you care about the precision of segmentation and do not want to cut audio based on the segmentation, `aligned_for_diar.stm` may be the right choice for you.
