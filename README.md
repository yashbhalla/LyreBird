LYREBIRD - VOICE-TO-TEXT NOTE MAKING SOFTWARE WITH SPEECH RECOGNITION

----------------------------------------------------------------------

Incorporates a Voice Classification AI Model capable of identifying and distinguishing between 15-20 people with 95% accuracy using only 60 seconds of audio per person as training data using Python and its modules.

Implements a Voice-To-Text feature that converts speech to text using AWS Cloud services and in conjunction with the Voice Classification AI, generates personalized transcripts of an audio clip detailing who spoke what.

The application incorporates the use of a Deep Learning Model. In order for the application to be able to identify speakers, it would require the data of each speaker’s voice in the form of a 60 second (approximately) audio clip and the speaker’s name. This data will be used to formulate the dataset, which in turn, will be used to train the deep learning model. This will be part of the first-time application setup and does not need to be repeated at the start of each meeting. The data of each speaker along with the trained model will be stored, so as to provide hassle-free meetings in the future.

We aim to deliver 95% accuracy in identifying the speakers and producing the transcripts, given there are no disparities in the provided dataset and there are no disrupting background noises
during the meeting. Since the dataset will be saved, upon the joining of a new speaker, the entire dataset need not be formulated again. Only the data of the new speaker is required, which will be
added to the existing database. However, this would require the model to be re-trained. If the above described procedure for the new speaker is not followed, the new unidentified speaker will be
labeled as “Unknown Person”. The transcript of the meeting would be generated at the very end as a reference for all the participants of the meeting

Technologies Used: Python, Machine Learning, Deep Learning, tensorflow, keras, librosa, pydub, pyaudio, soundfile, numpy, AWS S3 Buckets

Training data and ML Model Performance:
- 60 seconds of training data per person in a 30 people dataset gives a 100% accuracy. 2 clips per person (30 seconds each).
- 30 seconds gives 93% accuracy.
- 15 seconds gives 85% accuracy.

References:
- https://subscription.packtpub.com/book/big_data_and_business_intelligence/9781787125193/9/ch09lvl1sec61/identifying-speakers-with-voice-recognition

- https://towardsdatascience.com/voice-classification-with-python-4bec6856d06a (Recommended)