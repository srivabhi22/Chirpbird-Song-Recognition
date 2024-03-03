
# CHIRPBIRD SONG RECOGNITION USING DEEP LEARNING
This was a winter project offered by GDSC, IITK which involved usage of neural networks to classify the audios of different categories of birds.The issue tackled by this project is to automate the remote monitoring of bird populations. A detailed description is given below regarding this project.



## DATA COLLECTION

We used the [`Cornell Birdcall Identification`](https://www.kaggle.com/competitions/birdsong-recognition) dataset which was availabel on Kaggle. Some basic information about the dataset are:
- It was a dataset which comprised of around 264 unique bird codes and 213755 bird audios.
- The train data consisted of short recordings of individual bird calls generously uploaded by users of [`xeno-canto.org`](https://xeno-canto.org/).

## DATA PREPROCESSING
The data had a large number of audio files and along with that many other features like elevation, longitude, latitude, bird code, species and many more. Other than the features which were given to us in the dataset, we also extracted the features from the audios of the birds. 
To analyze an audio, there are many parameters. Some of them are:
- **MFCC (Mel-Frequency Cepstral Coefficients)**

- **Zero-crossing rate:** and many more....
The major ones have been covered up above. For further detail please visit: [`Features of Audio`](https://towardsdatascience.com/how-i-understood-what-features-to-consider-while-training-audio-files-eedfb6e9002b)

## FEATURE EXTRACTION
I plotted the mel spectrograms from the mfccs of different audios. The input data were the images of the mel spectograms into our neural network architecture.

## ARCHITECTURE
Transfer learning was used to incorporate the usage of the ResNet50 model which gave a very decent accuracy.
