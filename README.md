# EntrAI

EntrAI is a proof of concept application trying to make IA assistant as invisible as possible. The goal is to run AI model locally without Internet connection and without having to open any other windows.

# Usage

Run the Python script and let it running in the background. Open your favorite text editor such as Notepad and write your prompt. Copy your prompt to the clipboard and type `!cr`. Wait a few seconds for the AI starting generating the response and then, start typing random letters on your keyboard. The program should replace your random letters by the IA response.

Instead of copying the text to your clipboard, you can also take a screenshot of the prompt (Maj + Win + S on Windows). EntrAI will read the text automatically using Tesseract.

To stop the generation and disable keyboard intercept, type `!s`. To quit EntrAI, type `!q`. The program will intercept all your keyboard inputs until you type `!s` or `!q`.

The project is configured to reply in French but you can easily change the langage in the code. You can also use another AI model available on Ollama. The default model is `llama3.2:latest`.

## Disclaimer

This project is **ONLY** made for testing purpose and is **ABSOLUTLY NOT** made for cheating at an exam.
**PLEASE DO NOT USE IT TO CHEAT!!**

I will not be held responsible for any problem you could get into by using this program. Cheating is most often forbidden and you could be prohibited from passing exams.

## Platform support

EntrAI should work on Windows. I haven't tested it on Linux and MacOS yet.

Note that EntrAI may be flagged as a virus by some antivirus because it could be concidered as a keylogger.

## Install

1. Install Python 3.11 or newer.
2. Install Tesseract from https://github.com/UB-Mannheim/tesseract/wiki and add it to your path.
3. Install ollama from https://ollama.com/.
4. Install Python dependencies by running `pip install -r requirements.txt` in the current directory.


I will not provide an installer as this project is only for testing and is not intended to be use by students trying to cheat.

## How does it work?

EntrAI uses the Keyboard Python library to intercept keyboard events. When the user types `!cr`, it will read the clipboard content, give it to the IA and store the answer. It is now in writing mode. EntrAI will intercept all keyboard events and write the answer's current letter instead of the random letter.
