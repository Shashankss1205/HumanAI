# HumanAI

# Project Name
Automating Text Recognition and Transliteration of Historical Documents with convolutional - recurrent architectures

# Description
Transliteration of text from centuries-old works represents a research area that is underserved by current tools, such as Adobe Acrobat’s OCR. While these resources can perform text recognition from clearly printed modern sources, they are incapable of extracting textual data from early forms of print, much less manuscripts. This project will focus on the application of self-supervised AI models to recognize text in Spanish printed sources from the seventeenth century.

# Task Name:
RenAIssance Project Tests for Prospective GSoC 2024 Applicants

# Task: 
I have developed a model based on convolutional-recurrent architectures for optically recognizing text in the provided dataset. Over the past 2 weeks, I have built this architecture from scratch and implemented it successfully.

# Approaching the Task:
I followed a very systematic approach for solving the task allocated:
Research and Understanding: I began by exploring various articles and research papers related to Optical Character Recognition Models to understand their working principles thoroughly.

Data Preprocessing: I meticulously preprocessed the dataset to ensure that the input was in the desired shape, adhering to the specified requirements.

Image Generation: I created a Python function to generate images using the provided PDF files, ensuring accurate representation of the textual content.

Page Splitting: To facilitate better model performance, I split double-sided pages into single-sided ones, enabling focused training on individual pages.

Word-to-Image Mapping: Developing a Python function to map each word from the document to the corresponding image was crucial in generating training data.

Bounding Box Detection: I trained a bounding box detector based on the CRAFT model to accurately identify and extract words from the images.

Data Sorting: To prevent mis-matching during training, I implemented a sorting algorithm. I sorted the images vertically, grouped similar values together, and then sorted them horizontally.

Model Training: Finally, I trained my model on the dataset using the CNN-RNN architecture, incorporating the CTC loss function for improved performance.

# Evaluation Metrics
I evaluated the performance of my model based on the CTC (Connection Temporal Loss) metric, known for its effectiveness in character recognition tasks.

# Future endeavours
### 1) Implementation of Self-Supervised Models and Transformers: 
Incorporating self-supervised learning techniques and transformer architectures into the existing OCR model can enhance its ability to recognize and transcribe text accurately. By leveraging self-supervised models, the system can learn more robust representations of the input data, leading to improved performance on historical documents with varying styles and fonts.

### 2) Augmentation of Training Dataset for Enhanced Model Training: 
Expanding the training dataset by incorporating additional historical documents and diverse writing styles can significantly benefit the model's training process. By augmenting the dataset with annotated examples, the model can learn to generalize better and handle a wider range of textual variations commonly found in historical manuscripts. This approach will contribute to improving the model's accuracy and adaptability to different document types.

### 3) Fine-Tuning and Refinement of Model Architecture: 
I will do Continuous refinement and fine-tuning of the model architecture for optimizing its performance on specific tasks. Experimenting with different network architectures, optimizing hyperparameters, and fine-tuning model weights based on performance feedback will be crucial steps in enhancing the OCR system's accuracy and efficiency. 

Additionally, conducting thorough analysis and evaluation of the model's performance on various historical documents will provide valuable insights for further refinement and improvement.