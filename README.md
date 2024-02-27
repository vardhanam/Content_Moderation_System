
# Mistral-7B-Instruct-v0.2 Model README

This README provides documentation for a Python script utilizing the `mistralai/Mistral-7B-Instruct-v0.2` model with 4-bit precision loading via the `transformers` and `bitsandbytes` libraries. The script offers a content review functionality to identify violations of community guidelines within a given text.

## Description

The script is designed to load the `Mistral-7B-Instruct-v0.2` model using 4-bit precision. It sets up the necessary configurations and utilizes a tokenizer for processing the input content. The model generates responses to identify potential violations of community guidelines in the provided content. Additionally, a `gradio` interface is used to interact with the model through a web interface.

## Installation

Before running the script, ensure that you have Python installed on your system, and install the following dependencies:

```sh
pip install transformers bitsandbytes torch gradio accelerate
```

## Usage

To use the script, you need to import the necessary modules and set up the model and tokenizer as shown in the provided code. The `predict` function takes in a message and historical context and outputs the model's prediction.

A Gradio interface is also provided to run the model as a web service, which can be accessed through a browser.

## Web Interface

To launch the web interface, run the script, and navigate to the provided local server URL (by default `http://127.0.0.1:7860/`) in your web browser.

## Model Configuration Details

The model uses the following configurations for 4-bit precision loading:

- **Compute dtype:** `float16`
- **Quantization type:** `nf4`
- **Nested quantization:** `False` (can be set to `True` if required)

## Contributing

If you encounter any issues or have suggestions for improvements, please file an issue or submit a pull request on the repository.
