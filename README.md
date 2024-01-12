Translation between languages using OpenAI API. It supports pdf document as input. 

To run it using command line: 

#Set you api_key as an environment variable

export OPENAI_API_KEY="sk-xxx" 

python ai_translator/main_JR.py --model_type OpenAIModel --openai_api_key $OPENAI_API_KEY --file_format markdown --book tests/test.pdf --openai_model gpt-3.5-turbo --target_language Japanese

Note: This is based on the following work (https://github.com/DjangoPeng/openai-quickstart/tree/main/openai-translator) by Mr. Peng. Here the feature of translation to any target language is added.
