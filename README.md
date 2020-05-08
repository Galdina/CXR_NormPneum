# Pneumonia Image Classification with Deep Learning


![coverphoto.png](https://github.com/viviandng/flatiron-project-4/blob/master/images/xray.png)

Contributors: Alphonso Woodbury & Vivian Dang

### Items in Repository:

- README.md - a summary of the repository content

- /images - all images

- /data - all data files pertaining to the pediatric chest x-rays

- /presentation - PowerPoint and pdf files of the final presentation

  

### Prompt:
According to the [American Thoracic Society](https://www.thoracic.org/patients/patient-resources/resources/top-pneumonia-facts.pdf), Pneumonia is the world’s leading cause of death among children under 5 years of age, killing approximately 2,400 children a day causing it to be the number 1 most common reason for US children to be hospitalized. Although we have adequate treatment for it like our oral and IV antibiotics, IV fluids, oxygen and rehydration therapy, we must be able to detect it and treat it immediately to prevent long term complications and death. </br>

In this project, our goal is to train and build a deep learning model that can classify whether a given patient has pneumonia, given a chest x-ray image.



### Results:

We developed a baseline dense layer model that achieved 0.81 accuracy on our validation set. Aiming for a high recall and balanced F1, we used a Convolution Neural Network that achieved 0.88 recall and 0.93 F1. 

Additionally, we used Transfer Learning model DenseNet to boost our score; the result was 0.98 recall with 0.76 F1. 


### Dataset:

https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

- Train folder:
  - 1341 normal 
  - 3875 pneumonia 
- Val folder:
  - 8 normal 
  - 8 pneumonia 
- Test folder:
  - 234 normal 
  - 390 pneumonia 

### Methodology:

1.	Download the dataset 
2.	Reshape x-rays to  64x64 and create a baseline model with dense layers (fully connected)
3.	Train the data on different models and compare recall scores
4.	Test the data on the best model (highest recall score)



### Recommendations:

- Incorporate our model to IT softwares (ex: epic) in hospital settings to assist health professionals diagnose pneumonia patients
- Use our model under the supervision of a radiologist to enhance accuracy/recall to improve treatment outcomes which will increase hospitals' ratings and fundings. 

### Next Steps:

- Improve the current model with additional chest x-ray data from adult patients 
- Explore machine learning solutions that detects the cause of pneumonia (viral vs bacterial)

  