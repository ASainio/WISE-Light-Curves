WISE light curves of ultra cool dwarfs analyzed with Lomb-Scargle periodogram.

Known issues:
- Colormap contains only 20 colors and currently there are 23 epochs. Therefor some epochs use same color.
Epoch colors are added to visualize data scattering when plotting off-set and folded light curves.
This should visualize better positional outliers from epoch clustering and in folded lightcurves it should reveal that epochs are not clustered.

- Baseline is a guess based on where 65-values have most datapoints to cover. In symmetric attached eclipsing binary system it is possible that amount of datapoints on each magnitude is about the same and therefor faintest end could be guessed.

Examples Baseline guesses on multiple sources:

![[V1403_Orionis](https://example.com/image.jpg](https://github.com/ASainio/WISE-Light-Curves/blob/main/example_images/V1403_Orionis.png))
If eclipsing binary is detached or semi-detached guessing the baseline works well. However the curve-fit in use does not return best outcome. This lightcurve is from V1403 Orionis.


![CSS J090826.3+123648]((https://github.com/ASainio/WISE-Light-Curves/blob/main/example_images/CSS%20J090826.3%2B123648.png))
If the source is symmetrical contact-binary the curve fit works well, but guessing the baseline can be wrong because amount of datapoints is similar in both minimas and maximas. Note the wrong guess on W2.
This example is CSS J090826.3+123648. 






