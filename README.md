# HICH Image/Text (HICH-IT)
we introduce a new multimodal dataset in the medical field of hypertensive intracerebral hemorrhage(HICH), called as HICH-IT, which includes both textual information and head CT images.
# Related notes
The dataset only displays a part of the dataset. Due to patient privacy concerns, parts of this dataset are fictionalized. Some data are presented in the form of tensors.If you are interested in this data set and want to obtain the complete data set, please contact email:***
# Experiment
we use our image data using the U-net segmentation model. Due to the unique structure of the U-net model, which aids in capturing the contextual information of images, the left side of U-net is a deep convolutional network responsible for extracting image features. The right side involves an upsampling process that gradually restores the image resolution. Furthermore, U-net excels in handling detailed aspects of images, enabling precise segmentation of small structures within images, which is crucial for medical imaging.We utilized Python scripting to convert NIfTI format images into PNG format. Subsequently, the images were randomly divided into training and testing datasets in a 7:3 ratio to validate the efficacy of image data when utilized with the U-net model
![image](https://github.com/CYBUS123456/HICH-IT-Datasets/assets/154394829/b356dbbe-cc61-48d7-8414-ffbbe8e0e701)

We use our text data on a Named Entity Recognition(NER) model, Named Entity Recognition (NER) models represent a key task in natural language processing. The objective of NER is to automatically identify named entities in text and categorize them into predefined classes.We divided the text data into training, testing and validation sets. After training,the weight files were imported into the test and validation sets to evaluate the effectiveness of the text data
![image](https://github.com/CYBUS123456/HICH-IT-Datasets/assets/154394829/11835906-cd8b-4240-adff-0cc39c57b6ce)
# Related Literature
HICH Image/Text (HICH-IT): Comprehensive Text and Image Datasets for Hypertensive Intracerebral Hemorrhage Research
https://arxiv.org/abs/2401.15934
