Transfer learning using the AfSIS large-scale spectral library
================
Philipp Baumann
14 August 2019

Motivation
----------

Soil spectral libraries (SSLs) are becoming larger and more diverse. This implies a shift from more general machine learning approaches to transfer learning in order to maintain predictive accuracy in comparison to more local modeling. Transfer learning is a concept established in the mid-90ties, which is gaining popularity in various ML and deep learning application domains.

The African Soil information service AfSiS . QED is developing an excellent infrastructure for the a SSL together with wet chemistry measurements, where some data can be found [on this Amazon AWS cloud image](https://registry.opendata.aws/afsis/). The explorations shown here builds upon [this tutorial](https://github.com/qedsoftware/afsis-soil-chem-tutorial):

The spectroscopic community has so far tested two main types of transfer learning, with promising results:

-   Instance-based transfer learning: The resampling(RS)-Local algorithm
-   Deep (parametric) transfer learning:

Technical notes
---------------

``` bash
# Install packages in coda environment in terminal
conda env create -n afsis-transfer -f environment.yml
```
