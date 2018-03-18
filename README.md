# Project Title:

# Identify Patients and Health Care Workers Using Transfer Learning on a Pre-trained Convolution Neural Network¶

Author: Kelvin Tham Kum Hong

## Aim

There has been extensive research in leveraging on Deep Learning to train Convolution Neural Networks (CNN) that can predict the presence of objects, humans and scenes in images [1][2][3].
However, the results from these research cannot be applied directly to healthcare problems such as monitoring of falls, daily activities, hand hygiene compliance, and be of practical use.
This project propose to train a CNN with the ability to foremost detect and predict human bodies as doctors, nurses or patients, as the groundwork for building future healthcare monitoring applications. The model shall be trained using transfer learning on Resnet18.

## Conclusion and Future Work

The model achieved a highest overall accuracy of 93.75% and the predictive performance of the classes are as follows:
- Doctor Acc:90.48%
- Nurse Acc:88.89%
- Patient Acc:97.44%

Considering the reasonable accuracy of the model, the author suggests its deployment in the areas of potential applications (gathered from feedback from clinicians and nurses):
- Patient monitoring/ Community care – Falls, sleep, vitals, motion/activity (rehab)
- Presence of visitors with patients
- Drink/food intake of patients
- Hand hygiene

Future work
- Training of model with more images containing side and back profiles of doctors and nurses
- Leveraging on subject recognition methods such as YOLO to automate cropping of images
- Explore if transfer learning on other networks such as Resnet152 or Inception V3,V4 will give better results
- Extracting weights of last fully connected layer to manually fine-tune (provide greater emphasize on prominant features such as stethoscope for doctors and short sleeves for nurses etc)
