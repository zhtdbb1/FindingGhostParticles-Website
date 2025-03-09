---
title: "Conclusion"
layout: default
nav_order: 4
---
# Final Energy Spectrum

The main goal of this project is to combine our collective classification and regression models to predict a PSD (Pulse Shape Discrimination) label and energy label in order to compile a final energy spectrum. The final energy spectrum is compared with the ground truth analysis label and quantified using the distance between the values squared (MSE), to serve as performance metric for the models. The classification task combines all the models used to predict the four PSD labels such as: low AvsE (Current Amplitude vs Energy), high AvsE, DCR (Delayed Charge Recovery), and LQ (Late Charge). These individual PSD labels are combined to determine whether a waveform is from a signal particle or a background particle. The predicted energy label is a numerical value that is proportional to the incident particle. These two predicted results put together form an energy spectrum plot, which is a frequency plot depicting the energy of the particle in keV on the x-axis. The full energy spectrum of our models that uses the full data set can be seen in the image below.

<center><img src="assets/images/our_energy_spectrums.png" alt="Final Energy Spectrums" width="90%" height="90%"></center>

The full energy spectrum consists of all the waveform events (3.2 million), whereas the cut version depicts the events that survived the PSD cuts (1.2 million). The sharp steplike features in the energy spectrum produced above is a result of the data processing in the Majorana Demonstrator experiment. Comparing our full energy spectrum with the ground truth analysis labels, we are able to achieve an MSE of 8180.5285. Furthermore, in the paper *Neutrinoless Double Beta Decay with Germanium Detectors: 1026 yr and Beyond (D’Andrea et al., 2021)*, it is suggested that neutrinoless double beta decay occurs around the 2000 keV benchmark, which is an area where our models seem to perform very well as seen below. 

<center><img src="assets/images/full_spectrums.png" alt="Full Spectrums" width="90%" height="90%"></center>

Finally, looking at the cut energy spectrums, we can see that the graphs have a slightly less overlap compared to the full energy spectrum plot. However, we were able to obtain a lower MSE value of 5345.6242 between our cur energy spectrum and the cut ground truth spectrum suggesting that our model performs better on the data after the PSD cuts. However, when looking at the 2000 keV levels, it seems that there is a larger gap between our predictions and the ground truth labels indicating that our model actually performs worse when detecting waveforms for double beta decay. 

<center><img src="assets/images/cut_spectrums.png" alt="Cut Spectrums" width="90%" height="90%"></center>

# Conclusion

## Placeholder