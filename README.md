# MRI bassed-Alzheimer-stages-detection-using-Deeplearning
This project is based on **Early detection** of **neurodegenerative disease** ,I started by studying _"_what are the methods by which I can detect these disease_"_
so, I gather ideas on --
* Blood Biomarker
* MRI (Magnetic Resonance Imaging) scan
* PET (positron Emission Tomography) scan
# Blood Biomarker in **AD (Alzheimer Disease)**
***
Blood Biomarker is a measurable indicator in the body that indicates the disease state/level in our body. And the disease are likes (may responsible for AD) --
- _**1. Amyloid Beta (Aβ42 & Aβ40)**_
- _**2. Tau protein (Hyperphosphorylation -> Neurofibrillary tangles)**_
- _**3. Neurofilament Light chain**_ 
***


Then I studied hippocampal atrophy, ventricles and the limbic system mean, and which MRI/PET changes correspond
to early vs. progressive disease. I collected a labeled MRI dataset `(folders: "NonDemented", "VeryMildDemented", "MildDemented",
"ModerateDemented")` and then I resize them into three categories `(folders: "NonDemented", "MildDemented",
"ModerateDemented")`  and explored literature and benchmarks (ADNI, AD classification papers) to shape my project goals: build
an image-based classifier for Alzheimer stage detection and learn about blood/CFS biomarkers and how imaging relates to clinical progression.

***
# **MRI(Magnetic Resonance Imaging)** I used for the prediction of different classification's of Alzheimer 
***
steps:-

 _**1. collect the Dataset**_ 
 - **Dataset Source**: _kaggle:https://www.kaggle.com/datasets_
   
 _**2. Data Preprocessing**_

  - **Image Resizing**: _All MRI images were resized to a fixed size 224 × 224 pixels (pixels depending on your implementation)_
  - **Normalization**
  - **Label Encoding**
    
 _**3. Dataset Splitting**_
  - **Dataset divided into: Training Set, Validation Set, Testing Set (70%,20%,10%) (I used this ratio)**
    
 _**4. Data Augmentation**_
  
 _**5. Feature Extraction**_
   
 _**6. Forward Propagation**_
   
 _**7. Loss Calculation**_
   
 _**8. Backpropagation**_
   
 _**9. Weight Update**_
   
 _**10. Epoch-Based Training**_
   
 _**11. Model Evaluation**_
   
 _**12. Model Saving**_
   
 _**13. User Uploads MRI Image**_
   
 _**14. Preprocessing of Uploaded Image**_
   
 _**15. Prediction by CNN**_

***
# REASON WHY CHOOSE THIS(GIVEN) DATASET FOR MY PROJECT (AS PER THE PAPER DETAILS)
***
 _**1. Original Dataset**_
   - _The dataset used is the OASIS MRI dataset_
     
 _**2. File Conversion**_
  - _`.img` and `.hdr` converted into `.nii`_
  - Original Scanner(The Pipeline)

         ↓
         
         .img
         .hdr
         
         ↓
         
         NIfTI (.nii)
         
         ↓
         
         2D JPG
   
 _**3. 461 Patients**_
  -This is one of the best parts.
     Many Kaggle datasets only say: "Contains 6000 images." But this one tells you: `461 real patients` (which mean `~170 per slices`and all total `~80,000 MRI images`)That is much more scientifically meaningful.
   
 _**4. Slicing Along the Z-axis**_
  - _brain images were sliced along the z-axis into 256 pieces_
  - _slices 100–160 were selected_
   
 _**5. Classification**_
  -They mention:
   CDR values: It means labels are based on actual clinical diagnoses rather than arbitrary folder names.
  For example:
  
           | CDR | Class        |
         | --- | ------------ |
         | 0   | Non Demented |
         | 0.5 | Very Mild    |
         | 1   | Mild         |
         | 2   | Moderate     |

  
