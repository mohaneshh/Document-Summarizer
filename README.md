📄 AI-Based Document Summarization Using Hugging Face Transformers
Project Overview
This project is an AI-powered document summarization tool that can generate concise and coherent summaries of long PDF documents using the LaMini-Flan-T5 model from Hugging Face.
It provides an easy-to-use web interface built with Streamlit, allowing users to upload PDFs and instantly view the summarized output.

🔥 Features
Upload any PDF document through a simple web interface

Perform abstractive summarization (not just copying sentences but rephrasing them)

View original PDF and summary side-by-side

Lightweight, fast, and deployable locally

Built with LangChain, Hugging Face Transformers, and Streamlit

📦 Installation Instructions
Clone the Repository

```bash
git clone https://github.com/your-username/Document-Summarizer.git
cd Document-Summarizer```

```
Install Required Packages
'''pip install -r requirements.txt'''


The key libraries used:
streamlit
transformers
torch
langchain
pypdf
sentence-transformers

Model Checkpoint Setup

Important Note:
In this project, the LaMini-Flan-T5-248M model is downloaded and stored locally (in my system) for faster access and offline usage.
If you are running this project on your own machine, you must download or import the model:

Option 1: Download the model manually
Visit Hugging Face Model Hub - LaMini-Flan-T5-248M
Click Download and save the model folder to your local machine
Update the checkpoint path in the code:

checkpoint = "path/to/your/downloaded/model/folder"

Option 2: Load the model directly from Hugging Face
You can modify the checkpoint to load online:

checkpoint = "MBZUAI/LaMini-Flan-T5-248M"
This will automatically download the model when the code runs (requires internet).

🚀 Running the Project
After setup:

Run the Streamlit app:

'''streamlit run app.py'''


🛠️ Project Workflow
PDF Loading: Read documents using LangChain's PyPDFLoader.

Text Splitting: Split large text into manageable chunks using RecursiveCharacterTextSplitter.

Summarization: Pass text chunks into the LaMini-Flan-T5 model using Hugging Face’s summarization pipeline.

Display: Show both the original PDF and the AI-generated summary side-by-side using Streamlit.

✍️ Example Screenshot

PDF View	AI Summary
(You can add real screenshots later!)

📚 References
LaMini-Flan-T5-248M - Hugging Face Model

Hugging Face Transformers Documentation

LangChain Documentation

Streamlit Documentation

⚡ Future Improvements
Add multi-language support (e.g., French, Spanish PDFs)

Highlight keywords between PDF and Summary

Improve mobile responsiveness for better viewing

🙏 Acknowledgements
Special thanks to Hugging Face, LangChain, and Streamlit for providing incredible open-source tools to make this project possible!

📬 Contact
If you have any questions or suggestions, feel free to open an issue or contact me.
