# PsychIT

This is a Psychiatrist Chatbot model that has been fine tuned using QLoRA and Quantized using GGUF.

## Prerequisites

To running this project, please ensure that you have the following installed:

- Python 3.8 or Higher (3.10 is recommended)
- Pytorch 2.3.1 (CUDA)
- Cuda toolkit 11.8 or 12.1

## Installation

1. Clone this repository:
```bash
git clone https://github.com/Raditya-P/PsychIT-AI-Therapist.git
```

2. Navigate into this project directory:
```bash
cd PsychIT
```

3. Create virtual environment:
    - Using venv:
    ```bash
    python3 -m venv psychIT-env
    ```
    - Using conda :
    ```bash
    conda create -n psychIT-env python=3.10.*
    ```

4. Activate the virtual environment
    - Using venv:
    ```bash
    source psychIT-env/bin/activate
    ```
    - Using conda:
    ```bash
    conda activate psychIT-env
    ```

5. Install the project dependencies
```bash
pip install -r requirements.txt
```

6. Run the project
    - Text classifier (download the model below):
    ```bash
    flask run
    ```
    - Text generator
    ```bash
    python3 usage.py
    ```

7. If you are done, you can exit from the virtual environment with:
```bash
deactivate
```

## Addition

If you want to use ollama, you can download Quantized model below, copy and paste quantized model in the same directory as Modelfile, and run ollama using:
```bash
ollama create psychIT -f Modelfile
ollama run psychIT
```

## Models
- QLoRA model : https://huggingface.co/radityap/QLoRA-PsychIT
- Quantized model : 
- Text Classification model : https://huggingface.co/radityap/PsychIT-mental-detection