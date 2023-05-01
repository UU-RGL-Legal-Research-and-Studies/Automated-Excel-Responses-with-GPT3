# Automated-Excel-Responses-with-GPT3

This repository contains code for an Excel-GPT-3 interface that generates automated responses for prompts using OpenAI's GPT-3 API. It uses Gradio for input/output interface, making it easy to use even for non-technical users. This tool is useful for generating responses for a large number of prompts in an Excel file. 

You can use the repository in conjunction with the 'Search-Buddy' repository. The Search-Buddy repository enables to extract data from PDFs into an Excel. Since GPT3 contains a maximum length of about 4000 tokens, Search Buddy can help by extracting the already relevant text from the PDF into an Excel. This excel can in turn be read by chatgpt through this repository (i.e. 'Automated-Excel-Responses-with-GPT3').

**Installation**

To use this tool, you need to have Python 3 installed on your computer. You also need to install the required Python packages. You can do this by running the following command: 

pip install -r requirements.txt

**Usage**

To use the tool, simply run the following command:

python main.py

This will start the Gradio interface, where you can upload an Excel file containing prompts and generate automated responses using GPT-3. The resulting responses are added as a new column in the Excel file and saved as a new output file.

**Configuration**

To configure the GPT-3 API, you need to set your OpenAI API key as an environment variable called Open_AI_Key. You can get an API key by signing up for OpenAI's GPT-3 API.

You can also modify the GPT-3 configuration by changing the model_config dictionary in the gpt() function. This dictionary contains various parameters that control the behavior of the GPT-3 model, such as the temperature, maximum number of tokens, and frequency penalty.

**Contributing**

If you find any issues or have suggestions for improvements, please feel free to create an issue or submit a pull request.
