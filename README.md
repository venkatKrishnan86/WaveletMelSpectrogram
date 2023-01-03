# WaveletMelSpectrogram (WMel-S)
 This project is about exploring the combination of Discrete Wavelet Transform with the Mel Filter bank, to obtain a better feature for inputting into a Deep Learning model, which in this case is a LSTM.
 
**Important note**: We do not aim to obtain a very high accuracy but only compare the use of Mel filterbank on Spectrogram and on Wavelet coefficients

The model takes the inputs as the Approximate and the Detailed Coefficients obtained from one level of DWT. The model architecture is as follows - 

![model](https://user-images.githubusercontent.com/88517272/210361192-1f7ca39f-1113-4b30-847b-70fe58b11e2c.jpeg)

## Experiment 1
This experiment was to compare with and without Wavelets using only the low frequency data. We obtain more than 5% improvement in test accuracy.

## Experiment 2
This experiment was to compare Wavelet Mel-Spectrogram using the whole frequency range. We obtain a better accuracy for Haar, Db2, Db3 and Db4 as compared to using only Mel-Spectrogram as a feature.
