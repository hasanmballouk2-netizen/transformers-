# transformers-
from transformers import pipeline 
qa_pipeline = pipeline(     "question-answering",  
model="deepset/roberta-base-squad2" )
context = """ Transformers is a library created by Hugging Face. It provides thousands of pretrained models. """ 
result = qa_pipeline(     question="Who created Transformers?",     context=context ) 
print(result)
