# Voice Frequency Analysis and Speech Enhancement

This project focuses on two core signal processing tasks using MATLAB: speaker gender classification based on voice frequency characteristics, and speech enhancement through spectral subtraction. The implementation combines practical techniques in audio signal analysis, spectral feature extraction, and basic denoising algorithms.

## Contents

- Gender Classification from Voice Frequency
- Speech Enhancement via Spectral Subtraction
- Code Structure and Usage
- Sample Input and Output
- Dependencies and Requirements

## 1. Gender Classification from Voice Frequency

The first part of the system processes recorded voice samples to determine the speaker's gender. Human vocal frequency typically differs between males and females, and this project leverages that difference to make predictions.

Key steps include:

- Reading `.mp3` audio files
- Applying Fast Fourier Transform (FFT) to obtain spectral representation
- Computing the power spectrum to identify the dominant frequency
- Classifying voices based on predefined frequency thresholds

An automated function is provided that accepts a folder path containing audio files and returns a vector of predicted gender labels.

## 2. Speech Enhancement via Spectral Subtraction

The second part implements a basic speech enhancement algorithm based on spectral subtraction. The method aims to suppress additive white Gaussian noise (AWGN) from audio signals.

Implemented steps:

- Opening a clean `.wav` speech file
- Adding AWGN at different noise levels using MATLAB's `awgn` function
- Applying spectral subtraction to reduce noise
- Comparing results across varying signal-to-noise ratios

This section highlights the effectiveness and limitations of a straightforward denoising approach when applied to speech data.
