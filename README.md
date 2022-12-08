# Speech-emotion-recognisation

Detecting emotions is one of the most important marketing strategies in today’s world. You could personalize different things for an individual specifically to suit their interest. For this reason, we decided to do a project where we could detect a person’s emotions just by their voice which will let us manage many AI-related applications. Some examples could be including call centres to play music when one is angry on the call. Another could be a smart car slowing down when one is angry or fearful. As a result, this type of application has much potential in the world that would benefit companies and even safety to consumers.
 
 #The architecture of Speech Emotion Recognition on the Backend Side:
 
 
 ![image](https://user-images.githubusercontent.com/86097622/206391902-addf2f85-20bf-45cf-b488-ba22b31f851d.png)


It can be seen from the Architecture of the system, We are taking the voice as a training samples and it is then passed for pre-processing for the feature extraction of the sound which then give the training arrays .These arrays are then used to form a “classifiers “for making decisions of the emotion . 

So, for the training sample the big data set of voice of different emotions is needed. We searched in the web and found different sets of datasets some of them are mentioned below:

 Crowd-sourced Emotional Multimodal Actors Dataset (Crema-D)
 Ryerson Audio-Visual Database of Emotional Speech and Song (Ravdess)
 Surrey Audio-Visual Expressed Emotion (Savee)
 Toronto emotional speech set (Tess)
 But We use Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS).

# Reasons to choose RAVDEES: (Tapaswi)
It has got 2452 audio files, with 12 male speakers and 12 female speakers.
The utterances of the speech are kept constant by speaking only 2 statements of equal lengths.
It has 8 different emotions by all speakers.
The emotions are mentioned as:
Calm
Happy,
Sad,
 Angry,
 Fearful,
 Disgust,
 and Surprise, along with
a baseline of Neutral for each actor
#Each of the RAVDESS files has a unique filename. The filename consists of a 7-part numerical identifier (e.g., 02-01-06-01-02-01-12.mp4). These identifiers define the stimulus characteristics
Filename identifiers (Mohit Wadhwa, July 25, 2020)
Modality (01 = full-AV, 02 = video-only, 03 = audio-only).
Vocal channel (01 = speech, 02 = song).
Emotion (01 = neutral, 02 = calm, 03 = happy, 04 = sad, 05 = angry, 06 = fearful, 07 = disgust, 08 = surprised).
Emotional intensity (01 = normal, 02 = strong). NOTE: There is no strong intensity for the ‘neutral’ emotion.
Statement (01 = “Kids are talking by the door”, 02 = “Dogs are sitting by the door”).
Repetition (01 = 1st repetition, 02 = 2nd repetition).
Actor (01 to 24. Odd numbered actors are male, even numbered actors are female).
Filename example: 02-01-06-01-02-01-12.mp4 
Video-only (02)
Speech (01)
Fearful (06)
Normal intensity (01)
Statement “dogs” (02)
1st Repetition (01)
12th Actor (12)
Female, as the actor ID number is even.

#Multilayer perceptron classifier: (Tapaswi)
A multilayer perceptron (MLP) is a class of feedforward artificial neural network (ANN). The term MLP is used ambiguously, sometimes loosely to any feedforward ANN, sometimes strictly to refer to networks composed of multiple layers of perceptron’s (with threshold activation).

 Multilayer perceptron’s are sometimes colloquially referred to as “vanilla” neural networks, especially when they have a single hidden layer.

MLP Classifiers
The multilayer perceptron is applied for supervised learning problems. The multi-layer perceptron issued for the purpose of classification. The MLP is made to train on the given dataset. The training phase enables the MLP to learn the correlation between the set of inputs and outputs. During training, the MLP adjusts model parameters such as weights and biases in order to minimize the error. The MLP uses Backpropagation, to make weight and bias adjustments relative to the error. The error can be calculated in many ways.
