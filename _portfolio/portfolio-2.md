---
title: "Geane Tracking"
excerpt: "The codebase (primarily C++) for a track fitting algorithm utilizing <img src="https://render.githubusercontent.com/render/math?math=\chi^{2}"> minimization and error propagation.<br/><img src='/images/gm2_sampletrack.png'>"
collection: portfolio
---





I developed a track fitting algorithm and implemented it into a larger track reconstruction framework as one of the first members of the 'Tracking Team' on the Fermilab Muon Muon <i>g − 2</i> experiment. This track fitting algorithm essentially combines separate hits across a detector into a single fitted track. The track fitting algorithm then fits large amounts (TBs) of incoming data for many tracks with high fidelity to provide vital telemetry for the experiment, and is still in use today. The algorithm was developed and tested with Monte Carlo simulations, and statistically verified before its implementation into the larger framework and put into production. A separate repository containing the [`Documentation`](https://github.com/nkinnaird/Geane-Documentation) can be found which details the algorithm and it's implementation.


The main infrastructure and flow of the track fitting code is shown below, along with a sample fitted track that the algorithm was successfully applied to.


<p float="left">
  <img src="/images/gm2_trackingworkflow.png" height="225" />
  <img src="/images/gm2_sampletrack.png" height="225" />
</p>



<!-- <p float="left">
  <img src="https://github.com/nkinnaird/Geane-Documentation/blob/master/Images/TrackingFlow/NewGeaneFittingFlow.png" height="225" />
  <img src="https://github.com/nkinnaird/Dissertation/blob/master/KinnairdThesis/Body/Figures/TrackingFigures/Tracks/SampleTrack.png" height="225" />
</p>
 -->
