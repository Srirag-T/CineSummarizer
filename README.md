Key Components:
Imports:

StrOutputParser from langchain_core.output_parsers: Parses the output from the language model.
PromptTemplate from langchain_core.prompts: Creates a template for the prompt.
ChatOllama from langchain_ollama: Interface for interacting with the language model.
Summary from openai.types.responses.response_reasoning_item: (Note: This import is not used in the script).
Movie Information:

A multi-line string movie containing detailed information about "Marvel's The Avengers".
Main Function:

Prints "Hello World" to indicate the script is running.
Defines a summary_template string that outlines the structure of the prompt, asking for a summary and cast list of the movie.
Creates a PromptTemplate object summary_prompt_template using the summary_template.
Initializes a ChatOllama object llm with the model "llama3".
Chains the summary_prompt_template with the language model and the StrOutputParser to create a processing chain.
Invokes the chain with the movie information and prints the result.
Purpose:
The script is designed to generate a concise summary and cast list for the movie "Marvel's The Avengers" by leveraging a language model to process the provided movie information.
