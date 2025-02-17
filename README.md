# Urdu Nazam Generator

This project focuses on generating **Nazam** (a form of Urdu poetry) using a Deep Learning model. The model, built using **GRU (Gated Recurrent Unit)**, is trained on a dataset of Roman Urdu poetry to generate the next part of a Nazam based on the user's input.

## Features
- **Generative Model**: Uses a GRU model to generate the next part of a Nazam based on user input.
- **Roman Urdu Text**: The model is trained specifically on Roman Urdu poetry, enabling it to generate authentic poetic text.
- **Web Interface**: A Streamlit-based web app allows users to:
  - Input starting text to generate poetry.
  - View generation history.
  - Download generated poetry results.

## Project Structure
```
├── main.ipynb              # Jupyter notebook for training the GRU model
├── roman urdu poetry.csv   # Dataset of Roman Urdu poetry used for training
├── poetry_gru_model.h5     # Trained model, ready for use
├── training_history.pkl    # Stores training history (loss, accuracy)
├── word_encoder.pkl        # Tokenizer for text-to-token conversion
├── app.py                  # Streamlit app for poetry generation
├── poetry_history.json     # Stores generated poetry history
├── requirements.txt        # Dependencies for the project
```

## Requirements
Install the necessary Python libraries using pip:
```bash
pip install -r requirements.txt
```
This will install:
- `streamlit` - For the web interface.
- `tensorflow` - For the deep learning model.
- `numpy`, `pandas`, and `scikit-learn` - For data handling and processing.
- `keras` - For deep learning functionality.

## Setup
### 1. Prepare Dataset
Ensure you have the dataset file **roman urdu poetry.csv**, which contains two columns:
- `Poet`: Name of the poet.
- `Poetry`: Roman Urdu text of the Nazams.

### 2. Training the Model
- Open and run the **main.ipynb** notebook to:
  - Preprocess the data.
  - Train the GRU model.
  - Save the model (**poetry_gru_model.h5**) and tokenizer (**word_encoder.pkl**).
- The trained model and tokenizer are saved for future use.

### 3. Running the App
After installing the dependencies, start the Streamlit app using:
```bash
streamlit run app.py
```
This will:
- Allow input of Roman Urdu text for poetry generation.
- Display and download generated poetry results.

**You can also access the app online:** *Nazam Generator*

## Using the Model
- The trained model can be loaded for inference or further deployment as needed.

## Notes
- Ensure that the appropriate version of TensorFlow is installed for compatibility with your environment.
- The app can store up to **50 generated poetry entries** in **poetry_history.json**.

Enjoy generating beautiful Urdu Nazams! ✨

