---
title: "Precession Frequency Analysis"
excerpt: "The codebase (C++, C, bash) for a high precision frequency analysis project, and associated statistical and systematic evaluations, for the Fermilab Muon <i>g − 2</i> physics experiment.<br/><img src='/images/gm2_precessionresults_1.png'>"
collection: portfolio
---

*This project was done while as a graduate student and then postdoctoral research associate for the Fermilab Muon <i>g − 2</i> physics experiment. See extensive details in my [dissertation](https://github.com/nkinnaird/Dissertation).*


One primary component of the Fermilab Muon Muon <i>g − 2</i> experiment is the extraction of a specific, so-called 'precession' frequency from large amounts of data, PBs, to high precision (sub-parts-per-million). I was one of the lead analyzers for the first data-taking period of the experiment, and developed code for the analysis stage of this part of the experiment. To explain it simply (at the risk of underselling how much work was involved), I more or less fit 1D histograms with non-linear functions, and then conducted many statistical and systematic tests on those fits. I used a specific method called the "Ratio Method," which helped reduce systematic biases in the final fit results.


<!-- I also conducted many smaller Monte Carlo simulations in order to help develop my understanding of the real, sometimes messy, data in a clean environment. -->


The first image below shows fit residuals and the associated fast fourier transform (FFT) for one of the fits to the data. The most low-level fit contains five parameters, and as shown in the black FFT, leaves residual peaks indicating effects which are unaccounted for in the fit. The "Full Ratio Fit" in red on the other hand, included 14 fit parameters, and shows via the flat spectrum that all effects have been properly accounted for. The second image then shows the final (blinded) fits to the four datasets gathered in the first data-taking period of the experiment, where the precisions on the extracted frequncies are at the parts-per-million (ppm) level or smaller. The chi-squared values are included to show the goodness-of-fits, and each dataset is labelled by the informal moniker in the experiment.

<img src="/images/gm2_precessionresults_1.png" height="400"/>
<img src="/images/gm2_precessionresults_2.png" height="400"/>



<!-- <img src="https://github.com/nkinnaird/PrecessionFrequencyAnalysis/blob/master/PlotsForReadme/DatasetRatioFits.png" height="250" />
<img src="https://github.com/nkinnaird/PrecessionFrequencyAnalysis/blob/master/PlotsForReadme/FitResidualFFT.png" height="250" /> -->
