# Music Generator Project

This project is centered on the exploration of deep learning techniques for music generation. Using Long Short-Term Memory (LSTM) networks, the project demonstrates how machine learning can be applied to create music autonomously by learning patterns from a dataset of MIDI files.

## Technical Details
- **Neural Network Architecture:** The model uses LSTM layers which are highly effective for sequence prediction problems. This architecture helps in learning dependencies and patterns in musical notes.
- **Data Processing:** The musical data is first converted from MIDI files to a format suitable for the neural network, extracting sequences of notes and their timings.
- **Training:** The LSTM network is trained on these sequences, learning to predict the next note in a sequence based on the previous notes.
- **Music Generation:** After training, the model attempts to generate new music sequences starting from a seed sequence derived from the data set.
- **MIDI File Creation:** The output from the model is then converted back into a MIDI file, allowing the generated music to be played.

## Requirements
- Python 3.7 or newer
- TensorFlow
- Keras
- music21
- numpy

## Installation and Setup
1. Clone this repository to your local machine.
2. Ensure Python 3.7+ is installed.
3. Install the necessary Python packages:
   ```bash
   pip install tensorflow keras music21 numpy

## Customizing Music Data

To experiment with different types of music, you can replace the MIDI files in the Data folder with your own. The neural network will learn from any musical data provided, enabling the generation of music in a variety of styles.

## Usage

Open the Music_Generator.ipynb notebook in a Jupyter environment:

  1. Launch Jupyter Notebook:
     ```bash
     jupyter notebook
  2. Navigate to the Music_Generator.ipynb file and open it.
  3. Execute the cells sequentially to process the data, train the model, and generate music.
  4. You may also use the generated model by without training it using the last 2 cells of the notebook.

