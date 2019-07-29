# Medical Image Annotation Job

[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

TODO... OVERVIEW

## Preliminary observations…

1.	When I started scoping the project, the trigger question was “Is this a case of pneumonia…?”. However, after some reflection, I switched to “Does this x-ray image show the signs of pneumonia?”.
Classificators probably are not going to be Doctors, so answering to “Is this a case of pneumonia?” would suppose and undercover diagnosis. Also, given the shortness but powerful impact of the question (read it aloud) we could propitiate 2 biases:

    * Push classificators to unconsciously flag everything as pneumonia (in their minds just as a precaution)

    * Open the doors of the middle path selection, “Not sure”, as a way of avoiding imperatives. Related to bias and this label, “Not Sure” (thought for failing scenarios) for logical reasons we avoid any example given that we query against certainties reserving doubt just as the last instance to improve our job description, particularly tips and examples.
    
We want (as well) to keep the focus on the x-ray image and its interpretation, not try to “diagnose” nor give space to the human emotion or empathy (for the sake of the work, we should avoid any possible subjectivity).

2.	In relation to the labels I chose “Yes/No/Not sure”, maybe at future (and after more research) I would change their order. Why…? Well, the interpretation of cloudiness on x-rays could be a little tricky (it can get worse if we have a dataset with most of the cases flagged as “positives” and/or several “positives” in row)the instinctive first reaction could be to pick Yes since it is the first one and the one in repetition. 
