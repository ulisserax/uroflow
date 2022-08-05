# Uroflow
Machine Learning project to audio extraction and to develop a product to predict a prostatic problem in men through the uro flow rate test

# Audio Data handling using python

## Represented by parameters such as frequency, bandwidth, decibel, etc.
## An audio signal can be expressed as a function of amplitude and time.
Example of computer readable formats: wav, mp3, wma
Tools that can be used in python: Librosa and PyAudio
Spectogram: Visual way of representing the signal strength present in a wave. Through it we can see how energy levels vary over time and where you have more or less energy.
To analyze audio, we must extract what is relevant to the problem (Resource Extraction).
1. Spectral centroid: indicates at what frequency the energy of a spectrum is centered (the “center of mass” of the sound). Indicated to differentiate between noise, speech or music. It is the measure to show whether the spectrum contains a predominance of high or low frequencies.
2. Spectral Rolloff: measurement of signal shape. Represents the frequency at which high frequencies decline to zero
3. Spectral bandwith: defined as the light band size and integer size at its maximum half.
4. Zero-Crossing Rate: Simple way to measure signal smoothness to calculate oscillation. It has higher values for more percussive sounds like metal and rock. Often used to discern between voice and music. Vocal and non-vocal voices have low ZCR ratios, which means a wide variation in ZCR. In the case of songs, there is no significant variation in the ZCR rate.
5. MFCC: small set of features that describe the general shape of a spectral envelope.
6. Chroma Resource: 12 element vector indicating how much energy of each note is present in the signal. It allows a robust way to describe the measure of similarity between parts of songs.
7. STE (Short-Time-Energy): Quadratic temporal sequence of a data domain (sum of samples from a process window). It is a measure of the energy of a signal, often used to discern between music and speech. For speech, generally, STE has a great deal of variation compared to a song.
8. RMS (Root-Mean-Square): It is also a measure of energy in a sound signal (a more complex mathematical expression than STE - Square Root of STE/Number of Samples). Same idea to discern speech from music and with similar variations.
9. HZCRR (High-Zero-Crossing-Rate-Ratio): It is defined as the ratio of the number of graphic scenes whose ZCR is above 1,5 in 1 second.
10. LSTER (Low-Short-Time-Energy-Ratio): It is defined as the ratio of the number of graph scenes (graph regions) whose STE is below 0,5 in 1 second.
11. Spectrum Spread: It is closely related to the spectral centroid. It is the measure that signals whether the power spectrum is concentrated around the centroid or distributed along the spectrum. In the musical field, rock has a greater spectral power than calm music with flutes, for example.
12. Delta Spectrum: Differentiate between music and ambient sounds.
