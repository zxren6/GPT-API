To run (using command line inside Anaconda):

Open Anaconda Prompt, then type the following: 
1) cd   (check current path)
2) cd C:\Users\zxren\Documents\GitHub\openai-quickstart\langchain\openai-translator

3) run the following:

python ai_translator/main.py 

python ai_translator/main.py  --input_file tests/The_Old_Man_of_the_Sea.pdf

python ai_translator/main.py --model_type OpenAIModel --openai_api_key $OPENAI_API_KEY --file_format markdown --book tests/test.pdf --openai_model gpt-3.5-turbo --target_language Chinese

Or:

python ai_translator/gradio_server.py 



Note: 
1) OpenAI-API-key needs to be explictely given, e.g. in "main.py" and "gradio_server.py" and "flask_server.py", we add the following line:

**************
os.environ["OPENAI_API_KEY"] = "sk-xxx"
**************
