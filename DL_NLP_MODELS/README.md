# T5 and BART Models

This repository contains implementations of **T5** and **BART** models for summarizing medical reports. The goal is to convert unstructured data into structured summaries, providing insights in a user-friendly format. The project employs state-of-the-art Natural Language Processing (NLP) techniques and integrates libraries for efficient text extraction, processing, and model training.

---

## Models

### 1. **T5 (Text-to-Text Transfer Transformer)**

- **Purpose**: A versatile transformer model designed for sequence-to-sequence tasks such as summarization and translation.
- **Approaches**:
  - **Scratch Implementation**: Trained from the ground up to adapt specifically to medical text.
  - **Pre-trained Model Fine-tuning**: Leveraged pre-trained weights from Hugging Face to accelerate and optimize training.
- **Key Features**:
  - Text tokenization and preprocessing to suit medical language.
  - Customized training pipeline with gradient accumulation and extended epochs.

### 2. **BART (Bidirectional and Auto-Regressive Transformers)**

- **Purpose**: A transformer model that combines bidirectional (BERT-like) and auto-regressive (GPT-like) architectures, excelling in text generation and summarization.
- **Implementation**:
  - Fine-tuned using pre-trained weights from Hugging Face for medical report summaries.
- **Key Features**:
  - Evaluated using metrics like BLEU and ROUGE.
  - Capable of producing detailed, coherent, and concise summaries.

---

## Libraries and Frameworks

### 1. **Hugging Face Transformers**
- Used for both T5 and BART models.
- Facilitates pre-trained model integration, tokenization, and sequence-to-sequence tasks.
- Supports metrics like BLEU and ROUGE for evaluation.

### 2. **pdfplumber**
- Extracts text from medical reports in PDF format.
- Processes unstructured data into usable text for NLP.

### 3. **Pandas**
- Organizes extracted data into structured DataFrames.
- Enables manipulation and export to formats like Excel.

### 4. **NumPy**
- Handles missing values during preprocessing.
- Ensures data consistency for model training.

### 5. **PyTorch**
- Deep learning framework used for training T5 and BART.
- Efficiently manages GPU computations and model fine-tuning.

### 6. **scikit-learn**
- Evaluates model performance with metrics like accuracy and precision.
- Supports dataset splitting for training and testing.

---

## Summary

This repository showcases the integration of T5 and BART models with robust libraries for automating medical report analysis. The combination of pre-trained and fine-tuned approaches ensures accurate summarization, making medical insights accessible and understandable for end-users.
