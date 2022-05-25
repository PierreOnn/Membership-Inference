# Membership-Inference

### Background
The maritime transport is a complex system which is constantly in change1. 
Based on tracking mechanisms, a ship’s position and velocity could be identified to map the movements within waterways. 
With the help of this information, a classification task could be developed to determine the vessel type according to it’s characteristics and followed trajectory.
This provides a useful model to expose vessels that are performing illegal activities. 
For instance, a spoofed ship that carries out fishing in a restricted area. 
Although the information could be exploited for anomaly detection, it’s considered classified to ensure shipping company privacy.

### Research Method
The source of data will be AIS, which represents unique information about each moving vessel that is transmitted every minute. 
Past data is available for U.S. coastal waters for calendar years 2009 through September 20212. 
In specific, a total of 10 classes will be retained (e.g. cargo, tanker, towing, fishing, ...) to construct an informative probability vector. 
Moreover, as AIS data depicts a time-series, an LSTM architecture will be utilized for the target and shadow models to conduct research within membership inference.
