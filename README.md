# Medical QA Bot using Quantised GGUF Llama 2 LLM

This project implements a Medical Question-Answering (QA) Bot that leverages the quantised GGUF version of Llama 2 Language Model (LLM) downloaded from Hugging Face. The bot utilizes the Langchain library to work with the LLM. The information for the bot is extracted from a Gale Medicine Encyclopedia, which is then converted to vectors using a recursive character text splitter. The user interface (UI) of the project is built using Chainlit.

## Project Components

### 1. GGUF Llama 2 LLM (Quantised Version)

The project uses a quantised version of the GGUF Llama 2 Language Model, obtained from Hugging Face. This pre-trained language model serves as the core component for question answering and understanding medical queries.

### 2. Langchain Library

Langchain is a library used to interface with the LLM and facilitate interactions between the language model and the other components of the project.

### 3. Gale Medicine Encyclopedia

The Gale Medicine Encyclopedia is the primary source of medical information for the bot. The information is extracted and processed to create vectors that can be used for question answering.

### 4. Recursive Character Text Splitter

This component handles the conversion of the Gale Medicine Encyclopedia text into vectors. It recursively splits the text into characters and processes them to generate meaningful vectors.

### 5. UI using Chainlit

Chainlit is used to build the user interface of the project. It provides a seamless and interactive experience for users to input medical queries and receive answers from the bot.

### 6. Faiss (CPU)

Faiss (Facebook AI Similarity Search) is employed for efficient similarity search within the vector space generated from the Gale Medicine Encyclopedia.

## Setup Instructions

1. **Clone the Repository:**

   ```sh
   https://github.com/Md-Ali05/Medical-Bot.git
   cd medical-qa-bot
   ```

2. **Install Dependencies:**

   ```sh
   pip install -r requirements.txt
   ```

3. **Download Quantised GGUF Llama 2 LLM:**

   Obtain the quantised GGUF Llama 2 LLM from Hugging Face and place it in the appropriate directory within the project.

4. **Configure Langchain:**

   Configure the Langchain library to properly interface with the downloaded LLM and enable seamless interactions.

5. **Prepare Gale Medicine Encyclopedia Data:**

   Preprocess the Gale Medicine Encyclopedia data and run ingest.py to convert it to the required format for generating vectors.

6. **Run the Application:**

   ```sh
   python app.py
   ```

   Access the application through the provided UI to ask medical questions and receive relevant answers.

## Usage

1. Launch the application using `python app.py`.
2. Open the provided UI (Chainlit-based) in a web browser.
3. Input a medical question in the designated input field and submit the query.
4. The bot will process the question and provide an answer based on the information from the Gale Medicine Encyclopedia.


## License

This project is licensed under the [MIT License](LICENSE).
