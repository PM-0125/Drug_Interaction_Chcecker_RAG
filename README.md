# **Drug Interaction Checker**

## Overview
The **Drug Interaction Checker** is an interactive application designed to identify potential interactions between drugs, build a semantic knowledge graph, and provide concise, meaningful summaries of drug information. This project combines the power of Natural Language Processing (NLP), semantic data technologies, and deep learning-based summarization models to ensure safer medication use and better insights.

# **Disclaimer**
We have tried our best to keep the information Generic and precise Ground Truth available on  different authenticated platforms! However we do not claim 100% Accuracy and ground truth please consult to a Physician in any specific scenarios.

This tool is equipped with:
- **Natural Language Processing** for drug name recognition from user queries.
- **RDF Knowledge Graphs** for structured representation of drug data.
- **Hugging Face Transformers** for summarizing key information.
- **Multithreading** for faster data retrieval.

## Features
- **Drug Name Extraction**: Automatically extracts drug names from natural language queries.
- **Parallel Data Retrieval**: Fetches data about multiple drugs concurrently.
- **Knowledge Graph Construction**: Generates RDF graphs for drug interactions and related information.
- **Summary Generation**: Produces a clear, actionable summary using state-of-the-art language models.
- **Graphical User Interface**: Intuitive interface for entering queries and displaying results.


### How to Obtain the DrugBank XML File
To use this application, you need access to the `DrugBank.xml` file, which can be obtained from the [official DrugBank website](https://www.drugbank.com/):
- **For Students**: Sign up with your valid student ID.
- **For Professionals/Professors**: Use your institutional credentials for access.

If you face any issues obtaining the file or Running our Code or if you have any suggestions, feel free to contact us at **anjananandan0125@gmail.com**.


## Installation

### Prerequisites
- Python 3.7 or higher
- A running instance of the Apache Jena Fuseki server for RDF data handling (optional).

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/Drug-Interaction-Checker.git
   cd Drug-Interaction-Checker

2. **Set up a Python Environment Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate

3. **Install Dependencies Use the provided requirements.txt file to install dependencies:**
    ```bash
    pip install -r requirements.txt

4. **Run the Application Start the GUI application:**
    ```bash
    python Drug_Interaction_Checker.py


# **Usage**
1. Launch the application by running the script.
2. Input your query in natural language (e.g., "Can I take Aspirin and Paracetamol together?").
3. Click Submit and wait for the application to:
4. Extract drug names.
5. Fetch data from sources and construct a knowledge graph.
6. Summarize drug interaction insights.
7. View the Recommendation Summary displayed in the GUI.

# **Workflow**

1. **Data Pipeline**
    1. Input Processing: The user provides a query in natural language.
    2. Drug Name Recognition: The system identifies drug names using NLP.
    3. Data Retrieval: The application retrieves data for each drug from APIs and structured databases.
    4. Knowledge Graph Construction: An RDF-based knowledge graph is generated for drug interactions.
    5. Summarization: Key interaction insights are summarized using Hugging Face models.
    6. Output: Results are displayed in an easy-to-read summary in the GUI.

2. **Key Components**
    1. Knowledge Graphs: Built using rdflib and stored in Turtle (.ttl) format.
    2. Parallel Processing: Uses concurrent.futures.ThreadPoolExecutor for efficient data fetching.
    3. Summarization: Leverages Hugging Face's BART model for concise summaries.

3. **GUI**
    Interactive Interface: Built with tkinter to ensure ease of use.
    Status Updates: Keeps the user informed at every step of the process.


# **Contribution**
We welcome contributions to improve this project. Here's how you can contribute:

1. **Fork the repository.**

2. **Create a feature branch:**
    ```bash
    git checkout -b feature-name

3. **Push Your Branch:**
    ```bash
    git push origin feature-name


