# Personal-assistant-with-jac
A simple jac program that uses 'by llm' to implement a personal AI assistant that organises tasks and usee AI to generate responses.
##Features

Intent classification
Response generation
Text summarization
Keyword extraction

##Setup

#Install dependencies
pip install jaclang groq
Get Groq API key from "console.groq.com"

#Set environment variable
Linux/Mac/WSL
export GROQ_API_KEY="your_api_key_here"

# Windows PowerShell
$env:GROQ_API_KEY="your_api_key_here"

#Run
jac run assistant.jac

#Configuration
Edit the global LLM settings in the code:
jac glob llm = byLLM(
    model_name="groq/llama-3.1-70b-versatile",
    api_key=os.getenv("GROQ_API_KEY"),
    temperature=0.7,
    max_tokens=1000
);
#Add New Features
Just add methods with by llm:
jac can your_method(text: str) -> str by llm;

#Resources
'Jac Documentation'
'Groq Docs'
