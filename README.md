# Speech Recognition and Translation Application

This repository contains a Python-based application that uses speech recognition, translation, and text-to-speech technologies to recognize speech input from a microphone, translate it into a target language, and play the translated audio output.

## Features
- Captures audio input from the microphone.
- Recognizes the spoken text using Google Speech Recognition.
- Detects the language of the recognized text.
- Translates the text into a user-specified target language.
- Generates audio output for the translated text using Google Text-to-Speech.

## Prerequisites

Before running the application, ensure the following are installed:

1. Python 3.7 or later
2. Required Python packages:
   - `speechrecognition`
   - `googletrans==4.0.0-rc1`
   - `gtts`

You can install the dependencies using:
```bash
pip install SpeechRecognition googletrans==4.0.0-rc1 gTTS
```

3. A working microphone connected to your computer.

## Usage

1. Clone the repository:
```bash
git clone <repository_url>
cd <repository_directory>
```

2. Run the script:
```bash
python app.py
```

3. Follow the prompts:
   - Speak into the microphone when prompted.
   - Enter the target language from the supported list (e.g., Hindi, Tamil, Spanish).

4. The application will:
   - Display the recognized text.
   - Detect the language of the spoken text.
   - Translate the text into the target language.
   - Save and play the translated audio output.

## Supported Languages

The application supports translations into the following languages:
- Hindi
- Telugu
- Kannada
- Tamil
- Malayalam
- Bengali
- Spanish
- French
- German
- Italian
- Portuguese
- Russian
- Japanese
- Chinese
- Korean
- Urdu
- Arabic
- Turkish
- Greek
- Dutch
- Swedish
- Polish

## Output

The translated audio files are saved in the `outputs` directory, which is automatically created if it doesn't exist.

## Error Handling
- If the microphone is inaccessible, the application will display an error.
- If speech is not recognized, the application will prompt the user to try again.
- If translation or audio generation fails, the application will display appropriate error messages.

## Platform Compatibility
- **Windows**: Uses `start` to play audio files.
- **MacOS**: Replace `os.system('start')` with `os.system('open')`.
- **Linux**: Replace `os.system('start')` with `os.system('xdg-open')`.

## Contribution
Feel free to fork this repository and contribute by submitting pull requests.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Author
[Your Name](https://github.com/your-github-profile)

## Acknowledgements
- [Google Speech Recognition](https://pypi.org/project/SpeechRecognition/)
- [Google Translate API](https://pypi.org/project/googletrans/)
- [Google Text-to-Speech](https://pypi.org/project/gTTS/)

