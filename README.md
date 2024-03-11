# stts
https://gist.github.com/thomwolf/e9c3f978d0f82600a7c24cb0bf80d606


Speech-To-Text API
Description
This is a Simple API built using Python and FastAPI that converts speech to text using OpenAI's Whisper v3 Model from HuggingFace Transformers.

Installation
Clone the repository and navigate to the directory
git clone https://github.com/Arkapravo-Ghosh/speech-to-text.git
cd speech-to-text
Create a virtual environment
python -m venv .venv
Activate the virtual environment
Windows
GNU/Linux or macOS
Upgrade pip and install the dependencies
python -m pip install -U pip
pip install -r requirements.txt
Run the server
python main.py
Usage
Test with given sample audio file
curl -X POST -F "file=@./sample.webm" "http://localhost:5000/transcribe"
/transcribe (POST) - Transcribes the audio file sent in the request body and returns the transcript as a JSON response.