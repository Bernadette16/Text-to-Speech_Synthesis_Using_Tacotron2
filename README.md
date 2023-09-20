# Text-to-Speech with Various Models

This repository provides a Python script for converting text to speech using different models, including WaveRNN, Griffin-Lim, and WaveGlow. The script utilizes PyTorch and Torchaudio for text processing, Tacotron2 for text-to-spectrogram conversion, and WaveGlow for waveform synthesis.

## Getting Started

### Prerequisites

Before running the script, you need to have the following dependencies installed:

- Python (3.6+)
- PyTorch (1.9+)
- Torchaudio (0.9+)
- Gradio (2.0+)
- IPython
- Matplotlib

You can install these dependencies using pip:

```bash
pip install torch torchaudio gradio matplotlib
```

### Model Setup

The script uses pre-trained models for Tacotron2 and WaveGlow. WaveRNN and Griffin-Lim models are also included. Please ensure that you have the WaveGlow model downloaded and placed in the correct directory. You can download it from [this link](https://api.ngc.nvidia.com/v2/models/nvidia/waveglowpyt_fp32/versions/1/files/nvidia_waveglowpyt_fp32_20190306.pth).

### Running the Script

Run the script using Python:

```bash
python text_to_speech.py
```

This will launch a Gradio interface that allows you to input text and select the desired text-to-speech model (WaveRNN, Griffin-Lim, or WaveGlow). After entering the text and choosing the model, the script will generate and play the corresponding audio.

## Usage

1. Enter the text you want to convert to speech in the "Enter Text" textbox.

2. Select the desired text-to-speech model using the radio buttons:
   - **WaveRNN**: Uses WaveRNN for synthesis.
   - **Griffin-Lim**: Uses Griffin-Lim for synthesis.
   - **WaveGlow**: Uses WaveGlow for synthesis.

3. Click the "Submit" button to generate and play the audio.

## Acknowledgments

- This script leverages pre-trained models from NVIDIA's Deep Learning Examples repository.
- Gradio is used for creating the user-friendly interface.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
