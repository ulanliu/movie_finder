# Health-care assistant 

In today's fast-paced environment, patients often struggle to access timely medical advice due to long waiting times and the complexity of health systems. Many individuals face barriers such as appointment delays, geographical limitations, or lack of immediate access to healthcare professionals. 

This project aims to address this problem by developing a system that leverages Retrieval-Augmented Generation (RAG) technology to provide users with quick, accurate, and relevant medical advice based on their descriptions, bypassing traditional time and space constraints.

> **Important:** The advice given by the system is not a substitute for real medical therapy. Users are strongly encouraged to visit a doctor if they experience any health issues.


## Project overview
This is the RAG application built as a part of LLM zoomcamp.  
The Health-care assistant is designed to assist users to understand their body health.

The main use cases include:
1. The user has some medical question and want to qucik ask someone.
2. 


## Dataset

The dataset is from ruslanmv on [Hugging Face](https://huggingface.co/datasets/ruslanmv/ai-medical-chatbot), including:

- **Description**: The brief introduction of user's problem.
- **Patient**: The user's question.
- **Doctor**: The advise from ruslanmv's AI medical chatbot.

The dataset contains 257k records.

## Technologies

- Python 3.12
- Docker and Docker Compose for containerization
- OpenAI as an LLM
- Grafana for monitoring and PostgreSQL as the backend for it

## Evaluation Criteria

* ~~Problem description~~ (Done)
    * 0 points: The problem is not described
    * 1 point: The problem is described but briefly or unclearly
    * 2 points: The problem is well-described and it's clear what problem the project solves
* RAG flow
    * 0 points: No knowledge base or LLM is used
    * 1 point: No knowledge base is used, and the LLM is queried directly
    * 2 points: Both a knowledge base and an LLM are used in the RAG flow 
* Retrieval evaluation
    * 0 points: No evaluation of retrieval is provided
    * 1 point: Only one retrieval approach is evaluated
    * 2 points: Multiple retrieval approaches are evaluated, and the best one is used
* RAG evaluation
    * 0 points: No evaluation of RAG is provided
    * 1 point: Only one RAG approach (e.g., one prompt) is evaluated
    * 2 points: Multiple RAG approaches are evaluated, and the best one is used
* Interface
   * 0 points: No way to interact with the application at all
   * 1 point: Command line interface, a script, or a Jupyter notebook
   * 2 points: UI (e.g., Streamlit), web application (e.g., Django), or an API (e.g., built with FastAPI) 
* Ingestion pipeline
   * 0 points: No ingestion
   * 1 point: Semi-automated ingestion of the dataset into the knowledge base, e.g., with a Jupyter notebook
   * 2 points: Automated ingestion with a Python script or a special tool (e.g., Mage, dlt, Airflow, Prefect)
* Monitoring
   * 0 points: No monitoring
   * 1 point: User feedback is collected OR there's a monitoring dashboard
   * 2 points: User feedback is collected and there's a dashboard with at least 5 charts
* Containerization
    * 0 points: No containerization
    * 1 point: Dockerfile is provided for the main application OR there's a docker-compose for the dependencies only
    * 2 points: Everything is in docker-compose
* Reproducibility
    * 0 points: No instructions on how to run the code, the data is missing, or it's unclear how to access it
    * 1 point: Some instructions are provided but are incomplete, OR instructions are clear and complete, the code works, but the data is missing
    * 2 points: Instructions are clear, the dataset is accessible, it's easy to run the code, and it works. The versions for all dependencies are specified.
* Best practices
    * [ ] Hybrid search: combining both text and vector search (at least evaluating it) (1 point)
    * [ ] Document re-ranking (1 point)
    * [ ] User query rewriting (1 point)
* Bonus points (not covered in the course)
    * [ ] Deployment to the cloud (2 points)
    * [ ] Up to 3 extra bonus points if you want to award for something extra (write in feedback for what)

