# PyBot
Pybot is a sophisticated Python-based venture that aims to create interactive dialogue and provide insights by analyzing Python documents. By leveraging libraries and APIs in Python, Pybot likely enables users to interact with documents related to Python in a conversational manner. Pybot serves as a valuable tool for both learning Python concepts and retrieving specific information from Python documentation, thereby enhancing the overall experience of exploring and mastering the language.

# Installation
You can install the required dependencies using pip:\
pip install langchain   \
pip install openai==0.28\
pip install chromadb==0.3.29\
pip install tiktoken\
pip install pypdf

# Usage
**Document Loading:**  Pybot begins by gathering documents from a specified directory. It's capable of handling PDF files using PyPDFLoader, a tool for extracting text from PDFs.

**Text Processing:**  After loading, the documents undergo segmentation into smaller text portions for easier handling. This segmentation is achieved through RecursiveCharacterTextSplitter, which breaks down the text into manageable chunks.

**Embeddings Generation:**  Next, Pybot utilizes OpenAI's GPT model to generate embeddings for these text chunks. Embeddings capture the essence of the text's context, aiding in understanding and analyzing the content more effectively.

**Vectorization:**  The generated text chunks are then converted into vectors using Chroma, a specialized library for vector storage. This conversion enables efficient storage and retrieval of relevant information.

**Question Answering:**  Finally, Pybot sets up a conversational interface powered by OpenAI's GPT-3.5 model. Users can interact with the system by asking questions, and Pybot retrieves pertinent answers based on the processed documents, facilitating seamless and intuitive access to information.

# Workflow
<img width="676" alt="PyBot Pic" src="https://github.com/Varsini-P/PyBot/assets/122096025/6abfd401-3856-4526-88b1-607ac2954438">


