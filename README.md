Multimodal Audio-Visual Deepfake Detector (MAVDD)
We provide two options to use FakeAVCeleb Dataset:
1. Use our preprocessed data:
Audio files (train and test sets):
link to audio files: https://drive.google.com/drive/folders/1I1DyFD1OwAmEQ4u5pwxFPwIH6GU3qjwN?usp=sharing
Video frames (train set only):
link to video frames: https://drive.google.com/drive/folders/1JLnw20tJTnCEFb06XJAhZ08WepPNNa4s?usp=sharing
Video frames (test set only):
link to video frames: https://drive.google.com/drive/folders/1eL0kLlnK1SKI1ap5J6nYAAEueoqvsvh3?usp=sharing

2. Process your own data:
You can download FakeAVCeleb dataset from its official website : https://sites.google.com/view/fakeavcelebdash-lab/.
The dataset comprises videos categorized into RARV, FARV, RAFV, and FAFV, further organized into regional folders (African, South Asian, East Asian, European, and American), each containing videos of men and women. To begin, flatten the videos of each category into a single folder, then split the videos of the four categories into train and test sets. Subsequently, use our provided Jupyter notebook, Extraction_of_frames_and_audio.ipynb, to extract frames and audio from the videos.

We also describe how to use our approach:
Firstly you should install required libraries: Run the following command in your terminal to install the necessary Python libraries listed in our requirements.txt file:
pip install -r requirements.txt

Afterthat, you have two options:

1. Train and Evaluate the Models Yourself (Optional):
This option allows you to train and evaluate the models yourself using the provided jupyter notebooks:
Jupyter Notebooks Provided:

Train visual deepfake detection models using:
Xception_based_model_training.ipynb or
DenseNet_based_model_training.ipynb
Evaluate videos of the test set in the visual component only using:
Xception_based_model_evaluation.ipynb or
DenseNet_based_model_evaluation.ipynb
Train and evaluate audio deepfake detection models using:
MFCC_utilized_model_training_and_evaluation.ipynb or
Melspectogram_utilized_model_training_and_evaluation.ipynb
Evaluate videos of the test set in both visual and audio components using:
MFCC&Xception_Evaluation.ipynb
MFCC&DenseNet_Evaluation.ipynb
Melspectogram&Xception_Evaluation.ipynb
Melspectogram&DenseNet_Evaluation.ipynb
2. Use Pre-Trained Models (Recommended):
This is the recommended option for most users. You can directly evaluate our pre-trained models on your test videos. The model weights are available here: link to model weights: https://drive.google.com/drive/folders/11DfZtYY0qnV86Nb8HrjkuM3gASZNJTbe?usp=sharing.

Note: As mentioned in our paper, the Xception-based with MFCC-utilized models achieve the best overall performance in Audio Visual Deepfake Detection.
