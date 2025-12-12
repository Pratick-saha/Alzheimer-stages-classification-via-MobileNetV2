# Alzheimer-stages-classification-via-MobileNetV2
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
"ModerateDemented")` and explored literature and benchmarks (ADNI, AD classification papers) to shape my project goals: build
an image-based classifier for Alzheimer stage detection and learn about blood/CFS biomarkers and how imaging relates to clinical progression.
