WISE light curves of ultra cool dwarfs analyzed with Lomb-Scargle periodogram.

Hints:
- To get useable data of this set it would be advisable to use filters. Light curves are visually vetted and sources with "F" for given band should be discarded. However outliers migh remain in the sample. Another good filter is to set amount of datapoints >= 50 or >= 100. One might want to filter out low SNR and overluminous sources. 

Known issues:
- Colormap contains only 20 colors and currently there are 23 epochs. Therefor some epochs use same color. These are first epochs, most center epochs and last epochs.
- Light curves in first release aren't flattened by epoch before periodogram. There are cases where source moves from or towards brighter star and that causes epochs to be on different levels. This decision was made based on LS-periodogram testing on known sources. 
- Baseline is a guess based on what magnitude has most datapoints covering 0-hypothesis range. 

Improvements for future updates:
- Use SNR limit when running target list. It will save a lot of work when vetting results.
- Edit metadata posted on figures: SNR? Amount of original datapoints without filtering? PM? Remove W3 and W4?
- Print amount of epochs!

Examples:

![V1403_Orionis](https://github.com/ASainio/WISE-Light-Curves/blob/main/example_images/V1403_Orionis.png)

If eclipsing binary is detached or semi-detached finding the baseline works well. However the curve-fit does not return best outcome. The lightcurve above is from V1403 Orionis.

![CSS J090826.3+123648](https://github.com/ASainio/WISE-Light-Curves/blob/main/example_images/CSS%20J090826.3%2B123648.png)

With contact-binaries the curve fit works well, but guessing the baseline can be difficult. Note the wrong guess on W2.
Example above is CSS J090826.3+123648. 

![Alt text](https://github.com/ASainio/WISE-Light-Curves/blob/main/null-hyph.png)

Datapoints within range of null hypothesis, brighter and fainter counted. These are in catalog presented % totaling to 100%. Example is ASASSN-21qj where over 50% of datapoints are above the baseline indicating of brightening.








