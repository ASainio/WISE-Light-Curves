WISE light curves of ultra cool dwarfs analyzed with Lomb-Scargle periodogram.

Known issues:
- Colormap contains only 20 colors and currently there are 23 epochs. Therefor some epochs use same color.

- Baseline is a guess based on what magnitude has most datapoints. In attached eclipsing binary system it is possible that amount of datapoints on each magnitude is about the same and therefor faintest end could be guessed.

Examples:

![V1403_Orionis](https://github.com/ASainio/WISE-Light-Curves/blob/main/example_images/V1403_Orionis.png)

If eclipsing binary is detached or semi-detached finding the baseline works well. However the curve-fit does not return best outcome. The lightcurve above is from V1403 Orionis.

![CSS J090826.3+123648](https://github.com/ASainio/WISE-Light-Curves/blob/main/example_images/CSS%20J090826.3%2B123648.png)

With contact-binaries the curve fit works well, but guessing the baseline can be difficult. Note the wrong guess on W2.
Example above is CSS J090826.3+123648. 

![Alt text](https://github.com/ASainio/WISE-Light-Curves/blob/main/null-hyph.png)

Datapoints within range of null hypothesis, brighter and fainter counted. These are in catalog presented % totaling to 100%. Example is ASASSN-21qj where over 50% of datapoints are above the baseline indicating of brightening.








