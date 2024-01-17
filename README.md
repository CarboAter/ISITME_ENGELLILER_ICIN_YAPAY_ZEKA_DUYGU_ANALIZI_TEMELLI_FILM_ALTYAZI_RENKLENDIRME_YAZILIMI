# BADAN-v1.0.0

BADAN is a program dedicated to creating colored subtitles for movies or videos to enhance the experience of hearing-impaired individuals. It can be hard to understand the emotions conveyed in a scene for hearing-impaired individuals, especially if the characters' faces aren't clearly shown. This project aims to improve this situation by coloring the subtitles in accordance with the emotions conveyed.


# Requirements
Other than the external libraries stated in "requirements.txt" (keras, librosa, moviepy, numpy, openai, openai-whisper, pytube, pysrt, python-dateutil), this program requires FFmpeg to be installed to the system's PATH.

## FFmpeg Windows Installation
   - Download FFmpeg from [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html).
   - Add the path to FFmpeg to your system's PATH.

## FFmpeg MacOS Installation
   - Install Homebrew from [https://brew.sh/](https://brew.sh/).
   - Install FFmpeg using the following command: `brew install ffmpeg`


# Usage
The usage is pretty straightforward. Just download the files, enter your OpenAI API key to "ai.py" and run "main.py". Make sure that the files are on the same directories as they are in the repository.

## Language Selection
If you want to specify a language to Whisper, you can change `result = model.transcribe(audio)`to `result = model.transcribe(audio, language = "LANGUAGE_CODE")` in "ai.py".