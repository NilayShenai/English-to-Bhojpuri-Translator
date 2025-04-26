# English-to-Bhojpuri Translator

### Overview

This project presents a fine-tuned **mBART** model specifically designed for translating English text into Bhojpuri. Bhojpuri, as a low-resource language, has historically lacked large-scale machine translation resources. This work aims to bridge that gap by providing an end-to-end solution featuring a custom-built dataset and a fine-tuned multilingual model.

Access the deployed web application here:

- [Live Demo](https://huggingface.co/spaces/nilayshenai/English-to-Bhojpuri-Translator)

This project is inspired by previous work: [ENG-TO-BHOJPURI GitHub Repository](https://github.com/NilayShenai/ENG-TO-BHOJPURI).

### Image

![App Screenshot](https://raw.githubusercontent.com/NilayShenai/English-to-Bhojpuri-Translator/main/images/screenshot.jpg)

*Sample screenshot of the English-to-Bhojpuri Translator web application.*


### Key Components

- **Model:** [BART-English-to-Bhojpuri-Alpha2](https://huggingface.co/nilayshenai/BART-English-to-Bhojpuri-Alpha2)
- **Dataset:** [English-Bhojpuri Translation Dataset](https://huggingface.co/datasets/nilayshenai/English-Bhojpuri_Translation_Dataset)

### Highlights

- **First-of-its-kind Dataset:** A curated English-Bhojpuri parallel corpus developed specifically to support machine translation and language modeling for Bhojpuri.
- **Fine-tuned mBART Model:** Utilizes the "facebook/mbart-large-50" architecture, adapted through focused fine-tuning on the custom dataset to ensure contextually relevant translations.
- **Low-Resource Language Advancement:** Contributes to Bhojpuri's digital presence by providing a strong foundational model for further research and applications.
- **User-Friendly Interface:** Built using Gradio Blocks with customized styling for a clean, intuitive user experience.

### Technical Details

- **Base Model:** `facebook/mbart-large-50`
- **Fine-tuning Library:** Hugging Face Transformers
- **Frontend Framework:** Gradio
- **Hardware Utilized:** NVIDIA T4 GPU for model training

The model is configured with beam search (`num_beams=5`) to enhance the quality of generated translations. Maximum sequence length is set at 128 tokens to ensure efficiency without sacrificing translation quality.

### Intended Applications

- **Academic Research:** Facilitates research in low-resource language processing and translation studies.
- **Language Preservation:** Supports initiatives aimed at preserving and promoting the Bhojpuri language in digital spaces.
- **Content Localization:** Can assist in adapting educational, cultural, or informational content into Bhojpuri.

### Limitations and Future Work

- **Early-stage Performance:** As this is an Alpha release, the translations may sometimes exhibit literal interpretations or minor grammatical inaccuracies.
- **Dataset Scope:** Model performance is inherently tied to the diversity and size of the initial dataset. Expanding the dataset with more varied and context-rich data is a potential future direction.

