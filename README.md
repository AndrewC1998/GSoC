# GSoC

Over the past two years I have taken part in GSoC. The README.md file contains links to each of the repositories which will be continually updated. All the code as was is also contained in the repository.

# 2018

Over the summer, I was working with Professor David Matteson at Cornell University and Senior Lecturer Dr. Rebecca Killick at Lancaster University to implement a new R package: changepoint.online. Although this work officially ended in August, I have continued developing this project further and begun writing a paper documenting the findings from the summer. Further work, such as the development of online non-parametric changepoint detection is now in the process of being developed.

Throughout the summer I was using R, C++ and C to create the R package and was working from Lancaster University in an office with Ph.D. students. This opportunity meant I was working in an office where new Statistical research was being developed and this enabled me to learn about areas of Statistics that had not been covered by my degree’s curriculum.

A brief summary of the project is provided below: There are many R packages available for offline changepoint detection but, to the knowledge of myself and the mentors, only one for online change point detection (cpm). This package would implement traditional “resetting” methodology, which means once a change has occurred previous data is forgotten. This project would bring the accuracy benefits of the offline methodology to the online setting, allowing users to implement the state of the art offline methods in a computationally efficient manner for online use.

The repository can be found at: [changepoint.online](https://github.com/rkillick/changepoint.online)

# 2019 

Detecting changes in statistical properties of a time series is important in a large number of fields. A large amount of research has taken place considering changes in mean and variance in time series. However, a typical assumption is that the error process is independent. Similarly more and more users of existing packages, for example changepoint, are facing problems using real world data due to the dependence structures present. There are several methods available in the literature that are not available in open source code. This project plans to address this by adding this functionality to a popular CRAN package, changepoint.

The project implements several changes in second order structure algorithms including the commonly used AR(p) structure and changes in variance and autocovariance (rather than spectra) through the LSW model.

The Locally Stationary Wavelet (LSW) process can capture many dependence structures. Of particular interest in changepoint applications is the fact that a piecewise second order time series will have its structure encoded as piecewise constant sequences in the local wavelet periodogram - a feature noted by Cho and Fryzlewicz (2012). Consequently when using the LSW framework for changepoint methods we do not need to be prescriptive about the structure of the dependence beyond the requirements of the LSW definition. A barrier to the current implementation in wbsts is that the majority of practitioners are familiar with variance and autocorrelation but not necessarily spectral decompositions - let alone time-varying spectra. For this reason we are seeking to implement a method to detect changes in variance and covariance through the non-parametric LSW model instead of a change in spectra.

This years project ended up affecting several dependencies on other projects. Please read the news within each repository to see exact changes. The updated repositories can be found:

- [changepoint](https://github.com/AndrewC1998/changepoint)
- [changepoint.np](https://github.com/AndrewC1998/changepoint.np)
- [EnvCpt](https://github.com/AndrewC1998/EnvCpt)

# Other
For the most up-to-date changes please look at the respective repositories. Please look at the code on this repository if you wish to see the final GSoC submissions.
