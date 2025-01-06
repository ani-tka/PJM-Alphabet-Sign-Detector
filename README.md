# PJM-Alphabet-Sign-Detector

This project implements a detector for recognizing Polish Sign Language (PJM) alphabet signs using computer vision techniques. The detector uses MediaPipe for hand landmark detection and a machine learning model (RandomForestClassifier) for gesture classification. 

The solution was inspired and adapted from a YouTube tutorial, with modifications to support PJM-specific gestures.([link-to-youtube-video](https://www.youtube.com/watch?v=MJCSjXepaAM&t=1054s)).

![pjm_detector](https://github.com/user-attachments/assets/b9043105-4b09-4bf2-adaf-047ee525d0c3)
<sub> the GIF was created using outputs generated from this project, source for additional images: https://www.slownikpjm.uw.edu.pl/page/opjm<sub>


Originally, the dataset contained 100 images per class. I increased this to 500 images per class, resulting in a more extensive dataset for training and evaluation.
The dataset now covers 20 signs of the Polish manual alphabet.
# How It Works
1. Data Collection:
A script captures images of hand gestures for each PJM alphabet sign and saves them in a structured dataset
2. Feature Extraction: Hand landmarks are extracted using MediaPipe, and the data is processed into normalized coordinates.
3. Model Training: A machine learning model is trained on the landmark data to classify hand gestures.
4. Gesture Recognition: The trained model predicts the sign from real-time webcam input, displaying the recognized letter on the screen.
## License
This project is based on code from [Computer vision engineer] ([link-to-original-repo](https://github.com/computervisioneng)), licensed under the [MIT License] ([link-to-original-license](https://github.com/computervisioneng/sign-language-detector-python/blob/master/License)).
