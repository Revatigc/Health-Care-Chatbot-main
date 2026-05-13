# Health-Care-Chatbot

<img src="https://www.scnsoft.com/blog-pictures/healthcare/how-chatbots-and-ai-are-changing-the-healthcare-industry_1.png" alt="Healthcare Chatbot Image">

A rule-based keyword chatbot designed to provide quick answers to frequently asked questions in healthcare. This chatbot uses predefined rules to guide users through menu options, offering symptom diagnosis, prevention advice, and consultation recommendations. It operates 24/7 and can handle multiple queries simultaneously.

<img src="https://miro.medium.com/max/875/1*69vLXZCjrJwdXytj0CTSiQ.jpeg" alt="Chatbot Illustration">

## Features

- **Symptom Diagnosis**: Identifies symptoms for common conditions like common cold, fever, diabetes, depression, and asthma.
- **Prevention Advice**: Provides medicines, lifestyle tips, and suggested foods for prevention.
- **Doctor Consultation**: Offers links to online doctor consultation services.
- **Interactive GUI**: Built with Tkinter for an easy-to-use graphical interface.
- **NLP-Powered**: Uses Natural Language Processing with NLTK and TensorFlow for intent recognition.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/Health-Care-Chatbot.git
   cd Health-Care-Chatbot
   ```

2. **Install Python dependencies**:
   Make sure you have Python 3.7+ installed. Install the required packages using the provided requirements.txt:
   ```bash
   pip install -r requirements.txt
   ```

   Alternatively, install manually:
   ```bash
   pip install tensorflow keras nltk numpy pandas
   ```

   For Tkinter (usually included with Python, but if not):
   - On Windows: Tkinter is included.
   - On Linux: `sudo apt-get install python3-tk`
   - On macOS: Tkinter is included.

3. **Download NLTK data**:
   The code will download necessary NLTK data automatically, but you can do it manually:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('wordnet')
   ```

## Usage

1. **Train the model** (if needed):
   Run the training script to generate the model:
   ```bash
   python training_py.py
   ```

2. **Run the chatbot**:
   - For command-line version: `python chatbot_py.py`
   - For GUI version: `python gui.py`

3. Interact with the chatbot by typing symptoms or questions related to healthcare.

## How It Works

- The chatbot uses a neural network model trained on intents from `intents.json`.
- It processes user input using NLTK for tokenization and lemmatization.
- The model predicts the intent and responds with predefined responses.
- Supports diagnosis, prevention, and consultation for various health conditions.

## Project Structure

- `intents.json`: Contains the intents, patterns, and responses for the chatbot.
- `training_py.py`: Script to train the neural network model.
- `chatbot_py.py`: Command-line version of the chatbot.
- `gui.py`: Graphical user interface for the chatbot.
- `chatbotmodel.h5`: Trained model file.
- `words.pkl` and `classes.pkl`: Pickled data for words and classes.
- `Data_Analysis.ipynb`: Jupyter notebook for data analysis.
- `heart-disease.csv`: Dataset for heart disease analysis.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

PS: Please do not forget to drop a star if you like it!
