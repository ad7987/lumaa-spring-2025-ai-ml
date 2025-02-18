# movie Recommendation System

A content-based movie recommendation system that suggests films based on semantic similarity to user input. Built using sentence embeddings and cosine similarity.

## Features

- **Semantic Search**: Uses `all-MiniLM-L6-v2` sentence transformer model for embeddings.
- **Cosine Similarity**: Matches user queries with movie descriptions using scikit-learn.
- **Stopword Removal**: Preprocesses queries by removing English stopwords.
- **Threshold Filtering**: Only returns recommendations with similarity scores ≥ 0.3.
- **PrettyTable Output**: Displays results in a clean tabular format with ratings.

## Installation

1. **Clone Repository**
   ```bash
   git clone [https://github.com/yourusername/movie-recommender.git](https://github.com/yourusername/movie-recommender.git)
   cd movie-recommender
````

2.  **Create Virtual Environment**

    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/Mac
    venv\Scripts\activate  # Windows
    ```

3.  **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

    *Sample `requirements.txt`:*

    ```
    pandas>=1.3.5
    numpy>=1.21.4
    sentence-transformers>=2.2.2
    scikit-learn>=1.0.2
    prettytable>=3.4.1
    jupyter>=1.0.0
    ```

## Usage

1.  **Dataset Setup**
    Place `Top_1000_IMDb_movies_New_version.csv` in the project root.

2.  **Run Jupyter Notebook**
    Execute all cells in `Recommendation_system.ipynb`.

3.  **Input Query**
    When prompted, describe your preferred movie genre/theme:

    ```
    Tell me what kind of movie you're in the mood for: [your input]
    ```

4.  **View Results**
    System outputs top 5 recommendations with similarity scores and IMDb ratings.

## Dependencies

  - Python 3.8+
  - Libraries:
    ![PyPI](about:sanitized)
    ![PyPI](about:sanitized)
    ![PyPI](about:sanitized)

## Contributing

1.  Fork the repository
2.  Create a feature branch (`git checkout -b feature/your-feature`)
3.  Commit changes (`git commit -m 'Add some feature'`)
4.  Push to branch (`git push origin feature/your-feature`)
5.  Open a Pull Request