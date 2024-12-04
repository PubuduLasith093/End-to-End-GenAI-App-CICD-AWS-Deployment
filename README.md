# End-to-End Signal Processing Chatbot - Generative AI

This project implements a signal processing chatbot using Generative AI technologies. It integrates LangChain, GPT, Pinecone, and Flask, with a deployment pipeline leveraging AWS EC2, ECR, and GitHub Actions.

---

## How to Run Locally

### Clone the Repository
```bash
git clone https://github.com/<your-repo-name>.git
cd <your-repo-name> 
```

### STEP 01: Set Up a Virtual Environment
Create a Conda environment and activate it:

```bash
conda create -n genai python=3.10 -y
conda activate genai/
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

### STEP 03- Create a .env file in the root directory and add your Pinecone & openai credentials as follows:
```bash
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

# run the following command to store embeddings to pinecone
```bash
python store_index.py
```

# Finally run the following command
```bash
python app.py
```




