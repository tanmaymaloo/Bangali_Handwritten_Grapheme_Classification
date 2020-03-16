# Bangali_Handwritten_Grapheme_Classification
Bengali is the 5th most spoken language in the world with hundreds of million of speakers. It’s the official language of Bangladesh and the second most spoken language in India. Considering its reach, there’s significant business and educational interest in developing AI that can optically recognize images of the language handwritten. This work hopes to improve on approaches to Bengali recognition.

# About
for each image we need to provide 3 output i.e. **consonant_diacritic grapheme_root vowel_diacritic** therefore, for each prediction we made each model seperately so that for improving each output weights will change can't effect the accuracy of other output
**Accuracy** 
From resnet the Score Obtained is low i.e. .85 (because no unfreezing was done)
From densenet the Score Obtained is i.e. .936


# required Data
1. https://www.kaggle.com/c/bengaliai-cv19
2. https://www.kaggle.com/iafoss/grapheme-imgs-128x128 (can make it your own using code in inference ipynb file)
3. Models created from bangali_training.ipynb -> bangali-ResNet-FastAi.ipynb (**or**) bangali-dense-fastai.ipynb  
  1. https://www.kaggle.com/tanmaymaloo/saved-models (resNet saved-models)
  2. https://www.kaggle.com/tanmaymaloo/densenetmodel (densenet after Freezing unfreezing saved models)


# Files
There Is a file Name  
**bangali_training.ipynb (https://github.com/tanmaymaloo/Bangali_Handwritten_Grapheme_Classification/blob/master/bangali_training.ipynb) showing the complete process of**  
1. Using Transfer learning for models arc.
2. *Freezing and unfreezinh the layers of Arc.
3. choosing the appropiate LR
4. saving the Models

Other File such as **bangali-dense-fastai.ipynb**(https://github.com/tanmaymaloo/Bangali_Handwritten_Grapheme_Classification/blob/master/bangali-dense-fastai.ipynb) showing the inferense of the use of densenet121 as a TL and submittion   
File named **bangali-ResNet-FastAi.ipynb**(https://github.com/tanmaymaloo/Bangali_Handwritten_Grapheme_Classification/blob/master/bangali_ResNet_FastAi.ipynb) shoing the use of resNet34 as a TL and submittion  

# The Training and validation Accuracy For denseNet as followes for all the 3 model for each output

1. Dense-1  
epoch	train_loss	valid_loss	time  
-0	2.009743	1.587130	12:15  
-1	0.971630	0.711024	10:19  
-2	0.697952	0.505359	10:22  
-3	0.551502	0.431051	10:23  
-4	0.490617	0.413210	10:22  

2. UNFREEZ  
epoch	train_loss	valid_loss	time  
-0	0.419323	0.353437	11:05  
-1	0.247262	0.208286	10:58  
 
3. dense-2  
epoch	train_loss	valid_loss	time  
-0	0.471402	0.366688	10:25  
-1	0.252930	0.206714	10:24  
-2	0.177742	0.145115	10:30  
-3	0.145825	0.124715	11:04  
-4	0.134644	0.120527	11:17  
  
4. Unfreeze  
epoch	train_loss	valid_loss	time  
-0	0.121586	0.107282	12:17  
-1	0.100068	0.090788	11:57  
  
5. dense-3  
epoch	train_loss	valid_loss	time  
-0	0.401484	0.335572	10:32  
-1	0.213810	0.192496	10:29  
-2	0.175239	0.153521	10:20  
-3	0.146913	0.130607	10:15  
-4	0.134170	0.127403	10:22  
  
6. unfreez  
epoch	train_loss	valid_loss	time  
-0	0.218679	0.217679	11:00  
-1	0.109376	0.093467	11:02  
  
