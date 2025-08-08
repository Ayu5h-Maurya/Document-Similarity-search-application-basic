# Document Similarity Search App

A basic document similarity search application that uses OpenAI embeddings and cosine similarity to find the most relevant document from a collection based on a user query.

## 🚀 Features

- **Semantic Search**: Uses OpenAI's text-embedding-3-large model for generating high-quality embeddings
- **Cosine Similarity**: Implements cosine similarity to measure document relevance
- **Easy to Use**: Simple Python implementation with clear output
- **Scalable**: Can be easily extended to work with larger document collections

## 📋 Prerequisites

Before running this application, make sure you have:

- Python 3.7 or higher
- OpenAI API key
- Required Python packages (see Installation section)

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone <your-repository-url>
   cd document_similarity_search_app_basic
   ```

2. **Install required packages**
   ```bash
   pip install langchain-openai python-dotenv scikit-learn numpy
   ```

3. **Set up environment variables**
   Create a `.env` file in the project root and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   ```

## 📦 Dependencies

- `langchain-openai`: For OpenAI embeddings integration
- `python-dotenv`: For environment variable management
- `scikit-learn`: For cosine similarity calculations
- `numpy`: For numerical operations

## 🎯 Usage

1. **Prepare your documents**: Modify the `documents` list in `main.py` with your own document collection.

2. **Set your query**: Change the `query` variable to your search term.

3. **Run the application**:
   ```bash
   python main.py
   ```

## 📝 Example

The current implementation includes a sample with cricket-related documents:

```python
documents = [
    "Virat Kohli is an Indian cricketer known for his aggressive batting and leadership.",
    "MS Dhoni is a former Indian captain famous for his calm demeanor and finishing skills.",
    "Sachin Tendulkar, also known as the 'God of Cricket', holds many batting records.",
    "Rohit Sharma is known for his elegant batting and record-breaking double centuries.",
    "Jasprit Bumrah is an Indian fast bowler known for his unorthodox action and yorkers."
]

query = 'tell me about Virat kohli'
```

**Output:**
```
tell me about Virat kohli
Virat Kohli is an Indian cricketer known for his aggressive batting and leadership.
similarity score is 0.66
```

## 🔧 Configuration

- **Embedding Model**: Currently uses `text-embedding-3-large` with 300 dimensions
- **Similarity Metric**: Cosine similarity for measuring document relevance
- **Output**: Returns the most similar document and its similarity score

## 🚀 Future Enhancements

- Add support for larger document collections
- Implement document preprocessing and cleaning
- Add support for different embedding models
- Create a web interface
- Add batch processing capabilities
- Implement caching for embeddings

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

If you have any questions or issues, please open an issue in the repository.

---

**Note**: Make sure to keep your OpenAI API key secure and never commit it to version control. 
