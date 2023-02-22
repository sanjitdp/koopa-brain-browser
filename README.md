# koopa-brain-browser
Brain-computer interface (BCI) project for NeuroTechX organization at UCLA in 2023. Koopa is a web browser project using a steady-state visually evoked potential (SSVEP) with an electroencephalogram (EEG) device to enable web browsing using only brain signals. Koopa flashes non-standard shapes at varying frequencies across the screen to predict the user's next click.

## Question
Can we use a steady-state visual evoked potential (SSVEP) for fast prediction where the regions are non-standard shapes, which can be used to construct an application to aid in web browsing?

## Hypothesis
Visual stimulus from non-standard shapes will elicit a discernible signal collected via EEG, which can be used to construct an application to aid in web browsing.

## Measurable Metrics
We will keep track of performance for each type of shape used in experimentation and testing; this will allow us to see what shapes we can predict most efficiently. The proportion of correct and incorrect clicks made by the application with its predictive model allows us to analyze the accuracy of the model at identifying what a user is attempting to select on the screen. Furthermore, the information transfer rate (ITR) will be measured to ensure that the web browsing can be done conveniently and quickly.

## Experimental Design and Data Pipeline
* Write a web application to flash different parts of the screen and get data corresponding brain signals to where the flash is on the screen (localized prediction, not classifying into squares or regularized shapes).
* Equip group members with EEG, knowledge of strict procedure, and specific roles for experimentation.
* Get the data by allowing team members to use the web application while wearing an EEG. 
* Look at the data and check for errors in data collection or otherwise.
* Clean the data (look for outliers, missing values, etc.)
* Get relevant features from data by applying Fourier transform, high-pass filter, or other signal processing techniques.
* Try various predictive models (CNNs, RNNs, FNNs, VAEs, image segmentation models, generalized linear models, etc.)
* Use a variety of metrics to decide on a prediction model.
* Build a web browser using the predictive model to allow the user to interface with a computer using feedback to visual stimulus.
* If time allows, extend predictive model to try and  create a faster SSVEP-based keyboard with non-standard key regions.

## References
The following references are from recent papers on SSVEP-based web browsers with standard (rectangular) regions being flashed at different frequencies.

Camilleri, A., Porter, C., Camilleri, T. (2022). Boggle: An SSVEP-Based BCI Web Browser. In: Holzinger, A., Silva, H.P., Helfert, M., Constantine, L. (eds) Computer-Human Interaction Research and Applications. CHIRA 2020. Communications in Computer and Information Science, vol 1609. Springer, Cham. https://doi.org/10.1007/978-3-031-22015-9_6

A. Saboor et al., "A Browser-Driven SSVEP-Based BCI Web Speller," 2018 IEEE International Conference on Systems, Man, and Cybernetics (SMC), Miyazaki, Japan, 2018, pp. 625-630, doi: 10.1109/SMC.2018.00115.
