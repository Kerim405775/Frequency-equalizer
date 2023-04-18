# Frequency-equalizer
Equalization of the frequency of any signal, in this project for an audio signal

Frequency equalizer is a tool which allows to control frequency bands of an audio signal,
i.e. to boost or attenuate the signal in particular subbands. It can be realized using a
cosine-modulated filterbank by first performing analysis to decompose the signal into
subbands, then manipulating chosen components and combining them through
synthesis into modified version of the original signal. Prototype filters which ensure
perfect reconstruction (as used in the Filterbanks notebook) mostly have relatively short
impulse responses, therefore they are not suitable for this type of application where
steep slopes and high attenuation in particular subbands may be required. In this case,
prototype filters with quasi-perfect reconstruction property are preferred, as used in the
MPEG format (see attached literature, Tab. 18-4).
Based on cosine-modulated filterbank, design and implement frequency equalizer which
boosts/attenuates selected subbands. Analyze frequency responses of the analysis and
synthesis filters. Compare filterbank frequency response with and without equalization
procedure. Test your implementation on music audio file and compare the input with the
obtained results, e.g. spectra/spectrograms of the input and output audio files.
- Section 18.6. Implementacja programowa zespołu filtrów standardu MPEG
audio from “Cyfrowe przetwarzanie sygnałów : od teorii do zastosowań, WKŁ
2014” by T. P. Zieliński.
