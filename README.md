# Arabic to English Translator

A neural machine translation (NMT) system using a Transformer model to translate Arabic text into English. This project utilizes PyTorch for model implementation and Streamlit for the user interface.

## 📌 Features

- Translate Arabic text into English using a custom Transformer model.
- Custom tokenizer for efficient text encoding and decoding.
- User-friendly web interface using Streamlit.
- Supports GPU (CUDA) acceleration for faster inference.

## 🛠️ Installation

1. **Clone the repository:**

```bash
    git clone https://github.com/your-repo/ar-eng-translator.git
    cd ar-eng-translator
```

2. **Create a virtual environment (optional but recommended):**

```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. **Install dependencies:**

```bash
    pip install -r requirements.txt
```

4. **Ensure you have the model weights and tokenizer:**

   - Place `transformer_ara_eng_custom_tokenizer.pth` in the root directory.
   - Ensure `tokenizer.json` is also in the root directory.

## 🚀 Usage

1. **Run the Streamlit app:**

```bash
    streamlit run app.py
```

2. **Input Arabic text** and click on **Translate** to get the English output.

## 📚 Project Structure

```
├── app.py                # Main Streamlit app
├── tokenizer.json        # Custom tokenizer mappings
├── transformer_ara_eng_custom_tokenizer.pth # Trained model weights
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

## 🔍 How It Works

1. **Custom Tokenizer**
   - Loads a custom tokenizer from `tokenizer.json`.
   - Handles tokenization and detokenization with special tokens.

2. **Transformer Model**
   - Uses a 6-layer Transformer architecture with positional encoding.
   - Predicts token-by-token to generate translated text.

3. **Translation Pipeline**
   - Tokenizes the input text.
   - Generates the translated output by iterating through the decoder.

## 📊 Model Details

- **Architecture:** Transformer (6 layers, 8 heads, 256 hidden size, 1024 FFN)
- **Input:** Arabic text
- **Output:** English text
- **Framework:** PyTorch

## 📌 Dependencies

- Python >= 3.8
- torch
- streamlit

Install them via:

```bash
    pip install torch streamlit
```

## 🧪 Example

Input (Arabic):

```
مرحبا كيف حالك؟
```

Output (English):

```
Hello, how are you?
```

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

## 🤝 Contribution

Contributions are welcome! Feel free to submit a pull request or report issues.

## 📧 Contact

For inquiries, reach out at: ismailsarfraz9345@gmail.com

