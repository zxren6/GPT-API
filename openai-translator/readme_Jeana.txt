To run (using command line inside Anaconda):

Open Anaconda Prompt, then type the following: 
1) cd   (check current path)
2) cd C:\Users\zxren\Documents\GitHub\openai-quickstart\openai-translator
3) python ai_translator/main.py --model_type OpenAIModel --openai_api_key $OPENAI_API_KEY --file_format markdown --book tests/test.pdf --openai_model gpt-3.5-turbo
Or:
3) python ai_translator/main_JR.py --model_type OpenAIModel --openai_api_key $OPENAI_API_KEY --file_format markdown --book tests/test.pdf --openai_model gpt-3.5-turbo --target_language 中文

Note: 
1) OpenAI-API-key needs to be explictely given, e.g. in "openai_model.py", we add a line API_KEY = "...", and then use this variable API_KEY in the following script.

**************
API_KEY = "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"

class OpenAIModel(Model):
    def __init__(self, model: str, api_key: str):
        self.model = model
        # self.client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
        self.client = OpenAI(api_key=API_KEY)
...
**************
