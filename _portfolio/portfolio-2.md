---
title: "Geane Tracking"
excerpt: "Track-fitting algorithm utilizing chi-squared minimization and error propagation, for the Fermilab Muon <i>g − 2</i> physics experiment.<br/><img src='/images/gm2_sampletrack.png'>"
collection: portfolio
---

*This project was done while as a graduate student for the Fermilab Muon <i>g − 2</i> physics experiment. See extensive details in my [dissertation](https://drive.google.com/file/d/1svdQTMf3DBS_IxlBcKcXCyd4XHIo__C7/view?usp=sharing). The code base (primarily C++) for the project can be found [here](https://github.com/nkinnaird/GeaneTrackingCode).*


The Fermilab Muon <i>g − 2</i> experiment, for vital diagnostic and data analysis purposes, uses "tracking detectors" in order to measure where muons decay within the experiment. Muons decay to positrons, some of which then pass through these tracking detectors. The detectors themselves essentially consist of electrical devices which "light up" whenever a positron passes through them. One of the modules of the system can be seen below, where the silvery "straws" are the detectors which record discrete hits for incident positrons.


<img src="/images/Tracker.png" height="400"/>


As one of the first members of the 'Tracking Team,' I developed a track-fitting algorithm which fits hits from many separate positrons with various trajectories to unique tracks. This tracking algorithm was implemented into a larger track reconstruction framework, interfacing with upstream and downstream stages of the data pipeline. My algorithm has been used to process many TBs of data, and is still in use today. A separate repository containing the [documentation](https://github.com/nkinnaird/Geane-Documentation) can be found which details the algorithm and it's implementation, along with the testing and verification of it using Monte Carlo simulation. The main infrastructure and flow of the track-fitting code is shown below, along with a sample fitted track that the algorithm was successfully applied to.


<img src="/images/gm2_trackingworkflow.png" height="400"/>
<img src="/images/gm2_sampletrack.png" height="400"/>



<!-- I developed a track fitting algorithm and implemented it into a larger track reconstruction framework as one of the first members of the 'Tracking Team' on the Fermilab Muon Muon <i>g − 2</i> experiment. This track fitting algorithm essentially combines separate hits across a detector into a single fitted track. The track fitting algorithm then fits large amounts (TBs) of incoming data for many tracks with high fidelity to provide vital telemetry for the experiment, and is still in use today. The algorithm was developed and tested with Monte Carlo simulations, and statistically verified before its implementation into the larger framework and put into production. A separate repository containing the [`Documentation`](https://github.com/nkinnaird/Geane-Documentation) can be found which details the algorithm and it's implementation. The main infrastructure and flow of the track fitting code is shown below, along with a sample fitted track that the algorithm was successfully applied to. -->


<!-- <p float="left">
  <img src="https://github.com/nkinnaird/Geane-Documentation/blob/master/Images/TrackingFlow/NewGeaneFittingFlow.png" height="225" />
  <img src="https://github.com/nkinnaird/Dissertation/blob/master/KinnairdThesis/Body/Figures/TrackingFigures/Tracks/SampleTrack.png" height="225" />
</p>
 -->
