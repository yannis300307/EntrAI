# EntrAI

EntrAI is a proof of concept application trying to make IA assistant as invisible as possible. The goal is to run AI model locally without Internet connection and without having to open any other windows.

# Usage

Run the Python script and let it running in the background. Open your favorite text editor such as Notepad and write your prompt. Copy your prompt to the clipboard and type `!cr`. Wait a few seconds for the AI starting generating the response and then, start typing random letters on your keyboard. The program should replace your random letters by the IA response.

Instead of copying the text to your clipboard, you can also take a screenshot of the prompt (Maj + Win + S on Windows). EntrAI will read the text automatically using Tesseract.

The project is configured to reply in French but you can easily change the langage in the code. You can also use another AI model available on Ollama.

## Disclaimer

This project is **ONLY** made for testing purpose and is **ABSOLUTLY** not made for cheating at an exam.
**PLEASE DO NOT USE IT TO CHEAT!!**

I will not be responsible for any problem you could get with the program.
Cheating is forbidden by the law and you could be ban forever from all exams.

## Platform support

EntrAI should work on Windows. I haven't tested it yet on Linux and MacOS.

Note that EntrAI may be flagged as a virus by some antivirus because it could be concidered as a keylogger.

## Install

Install Python 3.11 or newer.
Install Tesseract from https://github.com/UB-Mannheim/tesseract/wiki and add it to your path.
Install ollama from https://ollama.com/.
Install Python Dependencies by running `pip install -r requirements.txt` in the current directory.


I will not provide an installer as this project is only for testing and is not intended to be use by students.