# langchain

# DataSlush Movie Recommendation Engine

## Overview

This project is a semantic search engine built using a movie dataset. It allows users to search for movies based on their preferences using a simple query input. The search leverages a pre-trained model from Hugging Face to generate embeddings and retrieves the most relevant movie matches using cosine similarity.

## Features

- **Data Extraction:** Reads movie data directly from a CSV URL without storing it locally.
- **Data Cleaning:** Cleans and preprocesses the data by handling missing values.
- **Text Embedding:** Uses a pre-trained model from Hugging Face to generate text embeddings for the movie features.
- **Vector Storage:** Stores embeddings in a vector database for efficient semantic search.
- **User Interface:** Built with Streamlit, allowing users to input search queries and get movie recommendations based on semantic similarity.

## Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Setup

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Create a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Run the application:

    ```bash
    streamlit run app.py
    ```

## Usage

1. **Load Data:** The application will automatically load and clean the movie dataset.
2. **Generate Embeddings:** The text embeddings will be generated using the Hugging Face model.
3. **Search:** Enter your movie preferences in the search bar, such as "heartfelt romantic comedy", and the app will return the most relevant movie suggestions.

## Project Structure

- `app.py`: Main application file.
- `requirements.txt`: List of Python dependencies.
- `README.md`: Project documentation.

## Model Details

The project uses the `sentence-transformers` library, which leverages a pre-trained model from Hugging Face for generating embeddings. The embeddings are then stored in a vector database, and cosine similarity is used for retrieving the most similar movies.

## License

This project is licensed under the MIT License.
