# MATLAB-Differential-Power-Analysis
 
This lab will introduce you to the basics of the DPA (Differential Power Analysis) - a technique that exploits the dependency of the<BR/> processed data on the power trace of the device to extract some secret information that would not be otherwise available. The goal is to learn how to process the power trace of the implementation of the AES encryption algorithm using an algebraic system (in our case Matlab) <BR/>and create the power hypothesis to extract the secret information (secret key of the AES). The entire lab can be found at<BR/>
https://rozvoj.fit.cvut.cz/Lisbon/Analysis

Task: Find the secret key.

At this point you are either given or were able to measure the power consumption (traces) of the smartcard yourself. For each power trace you have a pair of the plaintext and the encrypted ciphertext. Therefore you have all the information you need except the secret key. It is the goal of the differential power analysis to extract the secret key using the mentioned traces, plaintext, ciphertext and the knowledge of the encryption algorithm by creating the hypothesis of the power consumption and correlating it to the measured traces. 

Schedule
Plot one trace, check that it is complete.
Check the alignment of traces (they overlay correctly, triggering works).
Select the appropriate part of the traces (e.g. containing the first round). Read in the appropriate number of traces.
Depending on your measurements, you may have to perform a correction of mean values (if your measurements "wander" in voltage over time). You can do so by subtracting from each trace its mean value.
Recover the secret key using the DPA with correlation coefficients.
