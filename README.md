# ForensiCLIP: An Explainable VQA with DeepFake Document Forgery 

**INTRODUCTION**

The increasing sophistication of document forgery techniques has highlighted the need for advanced detection methods that can surpass the limitations of traditional approaches. 
Conventional systems, which primarily rely on Optical Character Recognition (OCR) and template matching, are increasingly vulnerable to modern forgeries capable of replicating security features and altering document layouts. 
These methods often lack adaptability to new forgery techniques while offering little to no explainability in their decision-making processes, an issue that significantly affects the forensic validation. 
To address these challenges, my project proposes an explainable Visual Question Answering (VQA) system using the CLIP model. 
My system is designed to detect anomalies of forgery while also providing some interpretable visual explanations which would enhance both the reliability and transparency of document verification.

**PROBLEM STATEMENT**

Forgery detection in documents has increasingly been difficult with the improvements in deepfake technologies. Traditional OCR-based systems often lack adaptability and fails in detecting certain anomalies. These anomalies are introduced via modern forgery techniques, such as inconsistent fonts, pixel artifacts, and/or misaligned signatures. Existing models provides absolutely no visual explanation for any decisions, which is a critical requirement in forensic science and security applications.

**PROPOSED SOLUTION**

+ My system utilizes OpenAI's CLIP model for multimodal feature extraction. 
+ The architecture consists of two primary components: the image encoder and the text encoder. 
   - The image encoder processes document images to extract visual features
   - The text encoder interprets forensic questions as textual prompts. 
+ These features are fused through element-wise multiplication to create a multimodal representation that is passed through a classification head for binary classification (genuine or forged). 
+ Visualization is integrated into the pipeline to generate outputs like graphs that highlight suspicious regions in the document, providing visual explanations for the model's predictions.
+ The Signature dataset is used as the primary source for training and evaluation. 
+ The system is expected to achieve high accuracy 75%+ in detecting forged documents while providing visual explanations that highlight anomalies such as signature mismatches or layout inconsistencies.
+ My proposed model is for now trained on signature dataset which consists of different handwritten and digital sign images which is focused on document forgery detection.
+ This model also includes visual explanations for forgery predictions by highlighting relevant regions in the document.

<img width="700" height="400" alt="image" src="https://github.com/user-attachments/assets/e50c998e-4732-4382-bd10-d9e0f0a96229" />

**IMPLEMENTATION**

<img width="700" height="400" alt="image" src="https://github.com/user-attachments/assets/c594b69e-a2ab-4590-a515-8118ff0491fd" />

**SUMMARY**

For this research my model successfully demonstrates an innovative approach to deepfake document forgery detection, by integrating models of CLIP and visualization to achieve  accuracy and interpretable results. By fine-tuning the CLIP model on the signature dataset and use of classification head tailored for forensic analysis, the system is capable of identifying anomalies in the forged document. The incorporation of visualization provides visual explanations, enhancing the trustworthiness and reliability of the system. The research also contributes to the advancement of document security by addressing the limitations of traditional methods and enabling more robust and transparent authentication processes. 

