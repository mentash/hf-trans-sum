# hf-trans-sum

NLP application for translating between multiple languages, I am using it to try English-German translations. It also summarizes long documents, and using open-source models from Meta using the transformers library from Hugging Face and PyTorch.

## Overview

HF-Trans-Sum is an NLP application that leverages open-source models from Meta, utilizing the Hugging Face Transformers library and PyTorch. The application provides two key functionalities:

1. **Translation**: Convert text between multiple languages
2. **Summarization**: Create concise summaries of long documents

## Environment Setup

### Prerequisites

- Python 3.8+
- Git
- Pip package manager

### Installation

1. Clone the repository:
   
```bash
   git clone https://github.com/yourusername/hf-trans-sum.git
   cd hf-trans-sum
```

2. Create and activate a virtual environment:

```bash
# Create virtual environment
python -m venv .venv

# Activate on Windows
.\.venv\Scripts\activate

# Activate on macOS/Linux
source .venv/bin/activate
```

3. Install required dependencies:

```bash
pip install -r requirements.txt
```

## Features

### Translation

- Powered by Meta's NLLB-200 model (No Language Left Behind)
- Converts between multiple languages with high accuracy
- Handles complex sentences and maintains context

#### Supported Languages

To choose other languages, you can find the other language codes on the Languages in FLORES-200 page.

For example:

- **Afrikaans**: afr_Latn  
- **Chinese**: zho_Hans  
- **Egyptian Arabic**: arz_Arab  
- **French**: fra_Latn  
- **German**: deu_Latn  
- **Greek**: ell_Grek  
- **Hindi**: hin_Deva  
- **Indonesian**: ind_Latn  
- **Italian**: ita_Latn  
- **Japanese**: jpn_Jpan  
- **Korean**: kor_Hang  
- **Persian**: pes_Arab  
- **Portuguese**: por_Latn  
- **Russian**: rus_Cyrl  
- **Spanish**: spa_Latn  
- **Swahili**: swh_Latn  
- **Thai**: tha_Thai  
- **Turkish**: tur_Latn  
- **Vietnamese**: vie_Latn  
- **Zulu**: zul_Latn  

### Summarization

- Condenses long documents while preserving key information
- Configurable summary length
- Supports various document formats

## Usage

The application can be used via the Jupyter Notebook interface:

1. Start Jupyter Notebook:

```bash
jupyter notebook
```

2. Open `trans-sum.ipynb` in your browser
3. Follow the code examples and documentation within the notebook

## Model Information

This project uses the following models:

- **Translation**: `facebook/nllb-200-distilled-600M`
- **Summarization**: `facebook/bart-large-cnn`

## Technical Details

- **Framework**: PyTorch  
- **Library**: Hugging Face Transformers  
- **Model Optimization**: Uses half-precision (FP16) to reduce memory requirements  

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
