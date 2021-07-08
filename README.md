# photometric-redshifts
Group Project for Artificial Intelligence Methods in Astrophysics in the WiSe 2020-21 at LMU Munich
Due to time constraints the project was implemented without any version control. Here we present the final results.

# Collaborators:

* Sebastián Gil
* David Rufer
* Qiang Wang (王强)

# Contents:

* Working Jupyter Notebooks at various stages of development
* Slides of Group Presentation in PDF Format

# Project Description:

The goal of this project was to predict photometric redshifts from observed images. The images are in jpg format and have
been prepared from SDSS fits images in the u, r, and g band. The file name for each images has the format
SDSSOBJID_z_REDSHIFTVAUE.jpg, where SDSSOBJID is the SDSS object ID, and REDSHIFTVAUE is the
spectroscopically measured redshift. The latter will be the label for each image, i.e. the machine learning algrorithms have
to be trained to reproduce this value for each image. The following non-exhaustive list contains suggested steps and
ideas to achieve reasonable results.
• Load the images and extract the label for each image
• Possibly crop and zoom the images (pipelines)
• Scale the pixel values (depending on the ML algorithms to between 0 and 1)
• Split the data in training, validation, and test sets
• Test different ML algorithms. You should use deep learning and at least 2 more commonly used methods, e.g.
random forests, SGD, SVM
• Think about regularization
• Plot learning curves - when do you stop?
• Determine the hyperparameters with the validation set
• What is the final score on the test set for each algorithm?
The data used can be found [here](http://www.usm.lmu.de/people/moster/Teaching/AI2020/projects/7_photoz_images/photoz_images.tgz)
