segment_evaluate
================

The token-based evaluation:
(1) Got the command variations from the generated cards (with space), and regarded them as gold standard;
(2) Concatenated all the space of the command variations, and used Chinese word segmentation package to get segmented command variations;
(3) Evaluated the Chinese word segmentation by the algorithm of the Edit Distance of the Word Separator, in which, substitution here represents good segmentations. Thus, the precision = (number of good segmentations) / (number of separators in all segmented segmentations); the recall = (number of good segmentations) / (number of all gold standard segmentations).

The results are as below,
Substitutions: 874410; Insertion: 7458; Deletions: 66549
Precision: 92.93%; Recall: 99.13%
