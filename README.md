# Medical-Chatbot

## Purpose:
The project aims to create a Medical Chatbot that uses **LangChain** for Natural Language Processing (NLP) and **Pinecone** for vector storage and retrieval. The chatbot is hosted on a **Flask** web application.

## Key Technologies Used:
1. **Flask**: Web framework for building the chatbot interface.
2. **LangChain**: Framework for building NLP chains, including retrieval-augmented generation (RAG).
3. **Pinecone**: Vector database for storing and retrieving embedded data.
4. **OpenAI**: Language model for generating responses.
5. **dotenv**: To manage API keys securely.
6. **Hugging Face Embeddings**: Pre-trained models for embedding textual data.

# How to run?
### STEPS:

Clone the repository

```bash
Project repo: https://github.com/Rohith1807/Medical-Chatbot
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n rmedibot python=3.10 -y
```

```bash
conda activate rmedibot
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```
### Create a `.env` file in the root directory and add your Pinecone & openai credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


```bash
# run the following command to store embeddings to pinecone
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```

### Acknowledgement
this project was inspired by Youtube tutorials by Euron.

# Conclusion
This Medical Chatbot project demonstrates the integration of cutting-edge NLP techniques using LangChain, OpenAI, and Pinecone within a Flask web application. By leveraging pre-trained embeddings and retrieval-augmented generation (RAG), the chatbot provides accurate and context-aware responses to medical queries.

This project not only showcases the practical implementation of generative AI in healthcare applications but also serves as a foundation for further enhancements, such as incorporating more robust medical datasets and fine-tuning response accuracy.
