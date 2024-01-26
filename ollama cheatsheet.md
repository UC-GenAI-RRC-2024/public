# OLLAMA
Ollama is an open-source LLM model manager. It provides a unified front-end for deploying 50+ popular open-source LLMs (including various flavors of llama2 and Mistral), simplifying the experience. 

## Links:
•	https://ollama.ai 
•	Great resources for general ollama use: https://github.com/jmorganca/ollama 
•	Ollama API: https://github.com/ollama/ollama/blob/main/docs/api.md 
•	Overview and setup: https://klu.ai/glossary/ollama 
•	Models/tags: https://ollama.ai/library 

## Install:
•	OSX or Linux
•	Local:
o	Download installer and run
o	Download or run curl https://ollama.ai/install.sh | sh

## Run:
•	ollama run <MODEL_NAME >:<TAGS>
•	Example; to pass a tag calling the 70 billion parameter llama2 model:
o	ollama run llama2:70b

## Pull a model:
•	Pull a model into local, without running it  
•	ollama pull <MODEL_NAME>:<TAGS>

## Copy a model:
•	Interacting with an LLM necessarily alters its training weights. We suggest copying the base model 
•	To copy a model: ollama cp <MODEL_NAME>:<TAGS> <NEW_MODEL_NAME>
•	To run a copy: ollama run <NEW_MODEL_NAME>

## Remove a model:
•	Pull a model into local, without running it  
•	ollama rm <MODEL_NAME>:<TAGS>

## Restore a mode to base:
•	ollama restore --model <MODEL_NAME>

## Stop server:
Pgrep ollama
>> <PROCESS_ID>>
Kill <PROCESS_ID>
