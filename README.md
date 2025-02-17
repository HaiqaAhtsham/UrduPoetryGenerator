# Generating Urdu Poetry with Deep Learning: A Streamlit-Powered AI Poet

## Introduction
Urdu poetry has a deep and expressive tradition, capturing emotions and thoughts in beautifully structured verses. With advancements in artificial intelligence, we can now generate poetic lines automatically using deep learning models. This article explores the development of an **Urdu Poetry Generator** powered by a **Gated Recurrent Unit (GRU) model** and a **Streamlit-based web interface**, making AI-generated poetry accessible to all.

## The Idea Behind the Project
The goal of this project is to create an AI poet that can generate Urdu poetry in **Roman Urdu**. The system allows users to:
- **Generate AI-written poetry** with a single click.
- **Customize poetry length and structure** to match their preferences.
- **Analyze generated poetry** for coherence and poetic elements.
- **Download poetry** for sharing or further refinement.

This interactive experience bridges technology and literature, bringing AI creativity to the world of Urdu poetry.

## Tech Stack & Implementation

### 1. **Dataset & Preprocessing**
The model is trained on a **dataset of Urdu poetry written in Roman Urdu**, sourced from public repositories and manually curated collections. Preprocessing involves:
- **Cleaning text** (removing special characters, handling stopwords, and normalizing variations).
- **Tokenization** (converting text into sequences for model training).
- **Padding sequences** to maintain consistent input lengths.

### 2. **GRU-Based Deep Learning Model**
We use a **Gated Recurrent Unit (GRU)** model, which is effective for text generation tasks due to its ability to capture sequential dependencies. The architecture includes:
- **Embedding layer** to convert words into dense vectors.
- **GRU layers** for sequential text learning.
- **Dense output layer** with a softmax activation to predict the next word.

The model is trained using categorical cross-entropy loss and the Adam optimizer.

### 3. **Building the Web Interface with Streamlit**
Streamlit provides an easy and interactive interface for users to generate and explore AI-generated poetry. The UI features:
- **A dark-themed interface** for a pleasant reading experience.
- **An input field** to specify poetry length and structure.
- **A history panel** to review previously generated poems.
- **A download button** to save poetry for offline use.

### 4. **Interactive Features**
Beyond just generating poetry, the app offers:
- **Poetry Analysis:** Identifies rhyme patterns and structure.
- **Customizable Generation:** Users can specify word prompts for AI-generated poetry.
- **Real-time Feedback:** Users can rate poetry for model improvement.

## Results & Performance
The trained model produces **coherent and stylistically relevant** poetry, capturing the essence of Urdu poetic structures. While it occasionally generates repetitive lines, fine-tuning and additional training data improve diversity and originality.

## Future Improvements
- **Fine-tuning on more diverse poetry styles** (e.g., Ghazals, Nazms, and modern free verse).
- **Incorporating Transformer models** like GPT or Llama for better contextual understanding.
- **Deploying the app** on platforms like **Streamlit Cloud or Hugging Face Spaces**.
- **Adding voice synthesis** for AI-generated recitations of poetry.

## Conclusion
This project showcases how **deep learning and NLP** can be leveraged to generate **creative text** in a culturally rich language. With further improvements, AI-generated poetry could become a valuable tool for writers, poets, and language enthusiasts looking to explore and experiment with Urdu literature.

Would you like to try it out? Let’s bring AI creativity to Urdu poetry together!

