# CB2330_Project_Group10
# Introduction
Our work is based on the data from the following paper:
Bagdonaitė L, Leder EH, Lifjeld JT, Johnsen A, Mauvisseau Q. Assessing reliability and accuracy of qPCR, dPCR and ddPCR for estimating mitochondrial DNA copy number in songbird blood and sperm cells. PeerJ. 2025 Apr 11;13:e19278. doi: 10.7717/peerj.19278. PMID: 40231068; PMCID: PMC11995889.

This paper compared the reliability and accuracy of dPCR and ddPCR to quantify low and high concentration of DNA using CVs. According to the paper, the concentration values of mtDNA from dPCR and ddPCR are estimated based on poisson statistics. 

However, we found that the ideal CVs are inconsistent with the observed ones using the ideal convention parameter. So we firstly constructed a generative model based on poisson distribution, and simulate the process of dPCR and ddPCR using Monte Carlo trials, then conducted the back forward process using ABC-MCMC method to find appropriate convention parameters.

# Implementation
Waiting for filling...

# Conclusion and Discussion
Conclusion:
On mechanical level, 1) we explained the physical source of the coefficient of variation in digital PCR and the mechanism of technical noise bias; 2) we proved that ddPCR has higher reliability and accuracy than dPCR especially at low concentration of DNA due to more partitions.
Discussion:
Model limitations: 1) 𝜃  is non-identifiable in biochemical level. Model couldn't identify different items contained in  𝜃 . 2)The assumption of treating experimental noise as constant proportionality could be inappropriate especially under super low dilution step, where most of the noise should be additive background noise. It may lead to model failure under low dilution steps.
