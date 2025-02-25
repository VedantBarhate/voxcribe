
# 🎙️ Voxcribe

Voxcribe is a Python package for transcribing audio files into text using speech recognition. It splits audio into manageable chunks, processes them in parallel, and combines the results into a single transcription.

---

## ✨ Features

- 🔊 **Supports Multiple Formats**: Works with MP3, WAV, and other audio formats.
- ⚡ **Chunk-based Processing**: Splits large audio files into smaller chunks for efficient processing.
- 🖥️ **Parallel Processing**: Utilizes all available CPU cores for faster transcription.
- 📊 **Optional Progress Bar**: Displays a progress bar during processing, which can be disabled if needed.

---

## 📦 Installation

Install Voxcribe using pip:

```bash
pip install voxcribe
```

### 🛠️ Prerequisites

Ensure the following dependencies are installed:
- [FFmpeg](https://ffmpeg.org/) (required by `pydub` for handling MP3 and other formats).

To install FFmpeg:
- **Linux**: Use your package manager (e.g., `sudo apt install ffmpeg`).
- **MacOS**: Use Homebrew (`brew install ffmpeg`).
- **Windows**: Download and install it from [FFmpeg's official website](https://ffmpeg.org/download.html).

---

## 🚀 Usage

### Example Code

```python
from voxcribe import Voxcribe

# Initialize the transcriber
transcriber = Voxcribe(chunk_duration=30, show_progress=True)

# Transcribe an audio file
result = transcriber.transcribe("audio.mp3")

# Print the transcription
print("Transcription:")
print(result)
```

### 🔧 Parameters
- `chunk_duration` (default: `30`): Duration of each audio chunk in seconds.
- `show_progress` (default: `True`): Whether to display a progress bar during transcription.

---

## 📋 Requirements

- 🐍 Python 3.6 or later
- 📜 Dependencies:
  - `speechrecognition`
  - `pydub`
  - `tqdm`

Install dependencies using pip:
```bash
pip install -r requirements.txt
```

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 💡 Acknowledgments

- 🔧 Built with the help of [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) and [pydub](https://pypi.org/project/pydub/).
- 📊 Progress bar powered by [tqdm](https://pypi.org/project/tqdm/).

---

## 📬 Contact

For issues or suggestions, feel free to:
- Open an issue on the [GitHub repository](https://github.com/VedantBarhate/voxcribe)
- 📧 Email me at `vedant.barhate27@example.com`
