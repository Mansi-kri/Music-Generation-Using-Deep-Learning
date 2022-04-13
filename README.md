
<h1>Music Generation Using Deep Learning</h1>

Sequence-to-Sequence model using multi-layered LSTM for music generation.
In this notebook, we will use LSTM, to build a character-based model that generates jazz piano notes.

Dataset

Music is available in a variety of digital audio formats ranging from raw audio (WAV) to more semantic representations such as MIDI (Musical Instrument Digital Interface), ABC, and sheet music. MIDI data already contains the information needed to feed the Deep Neural Network, we just need to transform it into an appropriate numeric representation to train the model. In next section discusses the details of this transformation.

For this work we will use the scale-chords dataset from here. Download the dataset (free small pack) that contains 156 scale chords files in MIDI format. Let's take a closer look at MIDI.

MIDI

MIDI is a communications protocol for electronic musical instruments. A Python representation of a MIDI file looks something like this:
![image](https://user-images.githubusercontent.com/66959193/163104662-3c5ab38c-605a-4b6d-9b9e-cf47c4a06e90.png)

From a higher-level perspective, the flow of data through the system looks like this:
![image](https://user-images.githubusercontent.com/66959193/163104754-2c2a5212-330a-4d95-95d8-b7ebce9b2444.png)



Required Libraries

We use the following libraries:

keras 

tensorflow

music21

pandas

numpy

pygame

timidity

