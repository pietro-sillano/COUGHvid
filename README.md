# COUGHvid
COVID-19 cough classification based on audio samples.

##s Dataset

The World Health Organization (WHO) has reported that 67.7% of COVID-19 patients exhibit a “dry cough,” which may be audibly different from
coughs caused by other pathologies. Such cough sounds analysis has proven successful in diagnosing respiratory conditions like pertussis,
asthma, and pneumonia. 
I employ the COUGHVID database [1], which is an extensive dataset of COVID-19  cough sounds from around the world, partially validated by expert pulmonologists.

## Feature extraction
I used a Convolutional Neural Network (CNN) for this task of classification. But why using a CNN if we're dealing with audio data ? Infact the first part of pipeline is to obtain a spectrogram of each audio sample. 
To create the spectrogram we use the Short Time Fourier Transform (STFT) that map our audio sample into the frequency domain.
A spectrogram is a visual way of representing the amplitude of the signal over time at various frequencies. Not only can one see whether there is more or less energy at, for example, 2 Hz vs 10 Hz, but one can also see how energy levels vary over time.
![plot](./img/spectrogram.png)

With the correct range of frequencies, STFT permit us to extract valuable and effective features from our data and fed into a standard CNN, since the spectrograms can be treated as images!
 

## Architecture
I choose to use pre-trained architectures to reduce training time and just fine-tuning the network weights. 

1. [EfficientNet](https://pytorch.org/hub/nvidia_deeplearningexamples_efficientnet/)
2. ResNet
3. Inception v3


## Results
<!--  confronto con una baseline di qualche tipo-->
TODO
## Future Work
TODO


# References
[1] Orlandic, L., Teijeiro, T. & Atienza, D. The COUGHVID crowdsourcing dataset, a corpus for the study of large-scale cough analysis algorithms. *Sci Data* **8,** 156 (2021). https://doi.org/10.1038/s41597-021-00937-4
[2] For downloading the dataset https://c4science.ch/diffusion/10770/
