  
![Featured Image - My PDF Talker](https://res.cloudinary.com/dkddubkcn/image/upload/v1720205321/1_mraqdy.png)

  
# Steps on how to run  
1) Create a Project Folder
```
mkdir <project-name>
```
2) Create a virtual environment and activate it
```
python -m venv .myenv
.\.myenv\Scripts\activate
```
3)  Install Required Dependencies
```
pip install langchain qdrant-client huggingface_hub sentence-transformers PyPDF2 cohere chainlit
pip install rank_bm25
pip install llama-cpp-python
```

4) Create a .env File with the Following Content Inside the Folder
```
[cohere]
api_key = Your COHERE API KEY1
```
You can obtain the API key by visiting: https://dashboard.cohere.com/api-keys

5) Download the Model Parameter File
```
zephyr-7b-beta.Q4_K_M.gguf
``` 
https://huggingface.co/TheBloke/zephyr-7B-beta-GGUF/blob/main/zephyr-7b-beta.Q4_K_M.gguf
Download the model file from the above link and save it to the current working directory.
  
6) Code Implementation
```
The code is inside the 'app.py' file.
```  
7) Run the server
```
chainlit run app.py
```
