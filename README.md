
# Text Generation using Recurrent Neural Network (RNN)

## Project Overview

This project demonstrates text generation using a Recurrent Neural Network (RNN). The model is trained on a text dataset and generates new text sequences similar to the input data. The implementation uses TensorFlow/Keras to build and train the RNN.

## Features

- Character-level text generation.
- Configurable sequence length and batch size.
- Model training with checkpoints to save progress.
- Text generation with customizable seed text and output length.

## Prerequisites

- Python 3.7 or higher
- Basic understanding of RNNs and neural networks.
- Familiarity with TensorFlow/Keras.

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/text-generation-rnn.git
cd text-generation-rnn
```

### 2. Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 3. Install the Required Packages
```bash
pip install -r requirements.txt
```

### 4. Download the Dataset
Download a text dataset (e.g., Shakespeare's works) and save it as `shakespeare.txt` in the project directory.

You can use the following command to download Shakespeare's works:

```python
import requests

url = "https://www.gutenberg.org/files/100/100-0.txt"
response = requests.get(url)
with open('shakespeare.txt', 'w', encoding='utf-8') as file:
    file.write(response.text)
```

## Usage

### Training the Model

To train the model, run:

```
text_generation_using_RNN.ipynb
```

This script reads the `shakespeare.txt` file, preprocesses the text, and trains the RNN model. Model checkpoints are saved periodically.

### Generating Text

To generate text using a trained model, use:

generate_text function which take 'seed' and 'length' as input
- `seed`: Initial seed text to start the generation.
- `length`: The number of characters to generate.

### Customizing the Model

You can adjust various parameters in the code:
- `seq_length`: Length of the input sequences.
- `batch_size`: Number of sequences processed in each training step.
- `epochs`: Number of training iterations.


## Acknowledgements

- [Project Gutenberg](https://www.gutenberg.org/) for providing free access to literary works.
- TensorFlow/Keras for the deep learning framework.

