
---  
title: '----'  
tags:  
  - Python  

authors:  
  - name: Mayukh Deb  
    orcid: ---  
    affiliation: 1  
  - name: Ujjwal Singh  
    orcid: ---  
    affiliation: 1  
  - name: Bradly Alicea  
    orcid: 0000-0003-3869-3175  
    affiliation: 1  
    
affiliations:  
 - name: OpenWorm Foundation  
   index: --  
date: -------  
bibliography: devolearn-joss.bib  
---  

# Summary
Extracting metadata from microscopic videos/images have been one of the key steps in the process of finding emerging patterns from various biological processes. There have been many attempts to develop segmentation tools for cell shape and location [1-3]. In particular, cell tracking methodologies provide quantitative summaries of cell centroid positions within an embryo [4].  Devolearn aims to speed up this process of collecting metadata by using robust deep learning models that can be used through a high level API. Devolearn’s primary focus is the _Caenorhabditis elegans_ embryo and specifically on the early embryogenesis process. Here are some of the capabilities of the DevoLearn model:

* segments images/videos of the _C. elegans_ embryo and extract the centroids of the cells and save them into a CSV file.  

* estimating the population of cells of various lineages within the _C. elegans_ embryo and upon user request generates plots of the data.  

* generating images of the _C. elegans_ embryo with a Generative Adversarial Network (GAN). The current version of DevoLearn (0.2.0) also supports bulk generation of images.  

DevoLearn has been made available as an open-source module, available on PyPi ([link](https://pypi.org/project/devolearn/)). All the deep-learning models used in devolearn are built and trained on PyTorch, the PyPI package (https://pypi.org/project/devolearn/) itself does not contain the model files, but the models are downloaded automatically once the user imports the model class from the package. 

## Statement of Need
Devolearn (0.2.0) is a python package that aims to automate the process of collecting metadata from videos/images of the C. elegans embryo with the help of deep learning models. This would enable researchers/enthusiasts to analyse features from videos/images at scale without having to annotate their data manually. 

There are a number of pre-trained models which are already in use in different contexts, but options are fewer within the unique feature space of developmental biology, in particular. Devolearn aims not just to fix this issue, but also work on other aspects around developmental biology with species-specific models. 

<P>
  <IMG SRC="https://github.com/DevoLearn/Education/blob/master/JOSS/DL-umbrella.png">
</P>

As a software ecosystem, Devolearn has been built to be very data science friendly and to be highly compatible with libraries like NumPy [5] and Pandas [6]. As the Devolearn ecosystem grows bigger with more tools and deep learning models, the combination of beginner friendliness and support for data science functionality will enable exciting scientific explorations both in developmental biology and data science. 

<P>
  <IMG SRC="----">
</P>

# Acknowledgements
We would like to thank the OpenWorm Foundation, the International Neuroinformatics Coordinating Facility (INCF), and Google Summer of Code for their financial and institutional support. Gratitude also goes to the DevoWorm group for their expertise and feedback.

# References
[1] Cao, J., Guan, G., Wong, M-K., Chan, L-Y., Tang, C., Zhao, Z., and Yan, H. (2019). Establishment of morphological atlas of _Caenorhabditis elegans_ embryo with cellular resolution using deep-learning-based 4D segmentation. _bioRxiv_, doi:10.1101/797688.

[2] Cao, J., Wong, M-K., Zhao, Z., and Yan, H. (2019). 3DMMS: robust 3D Membrane Morphological Segmentation of _C. elegans_ embryo. _BMC Bioinformatics_, 20, 176.

[3] Chen, L., Hang Chan, L.L., Zhao, Z., and Yan, H. (2013). A novel cell nuclei segmentation method for 3D _C. elegans_ embryonic time-lapse images. _BMC Bioinformatics_, 14, 328.

[4] Ulman, V. et.al (2017). An objective comparison of cell-tracking algorithms. _Nature Methods_, 14(12), 1141–1152.

[5] Harris, C.R. (2020). Array programming with NumPy. _Nature_, 585, 357-362.

[6] Virtanen}, P. et.al (2020). SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. _Nature Methods_, 17, 261-272.
