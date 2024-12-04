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

### STEP 03- Create a .env file in the root directory and add your Pinecone & openai credentials:
```bash
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

### STEP 04- run the following command to store embeddings to pinecone
```bash
python store_index.py
```

### STEP 05- Finally run the following command
```bash
python app.py
```

## Tech Stack Used

- **Python**: For backend programming and application logic.
- **LangChain**: To integrate and manage language model workflows.
- **Flask**: A lightweight web framework for serving the chatbot application.
- **GPT**: For generating human-like responses and powering the chatbot.
- **Pinecone**: Vector database for storing and retrieving embeddings.
- **AWS CI/CD Deployment with GitHub Actions**: Automates deployment processes, including building and deploying the chatbot application to AWS.

# AWS-CICD-Deployment-with-Github-Actions

### 1. Login to AWS console.

### 2. Create IAM user for deployment

```bash
#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess
```




