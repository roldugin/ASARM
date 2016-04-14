# Automatic Score Alignment of Recorded Music

[PDF version](https://raw.github.com/roldugin/ASARM/master/ASARM-ReportB.pdf)

## Abstract

The process of score-to-audio alignment matches the events in the score to the time when they occur in the audio recording. The results of the alignment can thus be used to time scale modify a musical piece or alternatively assign exact tempo at every position of the score, so that both are in sync with each other.

The method presented in this work uses a dynamic time warping technique with subsequent linear spline fitting to eliminate minor alignment errors and achieve a naturally sounding audio output.

The method has been designed with music notation software tools in mind. As such, it has performance optimisation as one of its goals. 

It is robust to errors in the score such as incorrectly transcribed notes. It does not make assumptions about the instruments present in either the audio recording or the score, but is targeted towards pop/rock music.

As opposed to methods that attempt to achieve a ground-truth alignment for indexing and machine training purposes, a new technique has been developed to prioritise the perceptional quality of the alignment.

A variety of methods at every stage of the alignment process are compared and discussed with reference to the problem at hand. In particular the chroma vectors will be presented as an alternative to pure spectral features.

The tests have shown them to be more stable than spectral features during rough alignments, but not as precise on the fine grained scale. The performance improvements result in a 70-90% reduction of the running time.

The obtained quality evaluation results show the validity of the approach and form the basis for a discussion of possible improvements to the process.
