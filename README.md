# PCP_project
OMTI and SECs processing code for Mesoscale Polar Cap Flows and their Impact on Polar Cap Patch Evolution

Abstract: 
Mesoscale convection in the high latitude ionosphere is known to exist, but how this convection impacts the propagation and evolution of ionospheric structures is still not well understood. We present a case study of two nights with polar cap patch activity, and examine the evolution of polar cap patches in relation to mesoscale flow structures using optical data from the Optical Mesosphere Thermosphere Imager All Sky Imagers located at Resolute Bay and Eureka, Canada, and high resolution convection maps from SuperDARN. We found that mesoscale flow channels are distinct structures in polar cap convection, and these flows changed on smaller spatial and temporal scales than the large-scale ionospheric flows and the patch lifetime. The polar cap patches responded to changes in the direction and strength of the mesoscale flow channels contained in the large-scale ionosphere flow patterns, often slowing down as the mesoscale flows ceased, or changed direction as other flow channels appeared. These results show that polar cap patch behavior is closely tied to mesoscale flow channels.

Notes on Project: 
We looked at two events, one with data from OMTI ASI at Eureka, Canada, and one from OMTI ASI at Resolute Bay, Canada. This pipeline could be used for other stations, but the time and pixel resolution would need to be changed within the code because information about those two stations is hard-coded in.
Secondly, this pipeline downloads data using PySPEDAS from OMTI and CDAWeb, so processing data using this code will require PySPEDAS and the supporting Python modules. This code also requires matplotlib, pandas, datetime, scipy, and numpy to be installed. 
Finally, the optical_calibrate function requires calibration files to be downloaded, which can be done here: https://stdb2.isee.nagoya-u.ac.jp/omti/stations.html#calibration 
This pipeline also requires radar SECs data to be downloaded, and aacgm coordinates to be downloaded. The conversion from pixel to magnetic latitude is not done in this pipeline. 
