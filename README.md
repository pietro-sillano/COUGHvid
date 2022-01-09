# COUGHvid
COVID-19 cough classification based on audio samples.


## Methods
I used a Convolutional Neural Network (CNN) for this task of classification. But why using a CNN if we're dealing with audio data ? Infact the first part of pipeline is to obtain a spectrogram of each audio sample. The spectrograms can be seen and treated as images.
To create the spectrogram we use the Short Time Fourier Transform (STFT) that map our audio sample, a time domain signal in the frequency domain.

![plot](../img/spectrogram.png?raw=true)




<!--# Table Of Contents
-  [In a Nutshell](#in-a-nutshell)
-  [In Details](#in-details)
-  [Future Work](#future-work)
-  [Contributing](#contributing)
-  [Acknowledgments](#acknowledgments)-->


# Dataset

The World Health Organization (WHO) has reported that 67.7% of COVID-19 patients exhibit a “dry cough,” which may be audibly different from
coughs caused by other pathologies. Such cough sounds analysis has proven successful in diagnosing respiratory conditions like pertussis,
asthma, and pneumonia. 
I employ the COUGHVID database [1], which is an extensive dataset of COVID-19  cough sounds from around the world, partially validated by expert pulmonologists.

# Future Work
TO-DO


# References
[1] Orlandic, L., Teijeiro, T. & Atienza, D. The COUGHVID crowdsourcing dataset, a corpus for the study of large-scale cough analysis algorithms. *Sci Data* **8,** 156 (2021). https://doi.org/10.1038/s41597-021-00937-4
[2] For downloading the dataset https://c4science.ch/diffusion/10770/
