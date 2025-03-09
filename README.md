This is a sql genration code leveraging llama 3 - 8B model 

The code also used chromadb vector database to store tables description
  
    This will be passed on as additional context to the llm 

Special instructions are also provided in the prompt to make it more accurate.
  
    For example if continent is passed on, llama will be able to modify that for countries as well 


Steps to be take to make it production ready 
  
    Introduce guradrails for the llm models -- For security 

    Pass historical query at a user + session level to chromadb -- This will be used as an additional context for the llama model.  
  
    If the number of query at a user + session level is more than threshold, then create mechanism to store them in a log file -- This can be further used to finetune the model 


