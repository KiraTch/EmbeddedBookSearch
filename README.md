# 📚 AI-Powered Book Recommender

An intelligent book recommendation system that uses Google's Gemini AI and semantic embeddings to help you discover your next favorite read from a vast collection of books.

## 🌟 Features

- **Semantic Search**: Uses AI embeddings to understand the meaning behind your preferences
- **Smart Query Processing**: Interprets natural language requests like "funny books about magic"
- **Genre Detection**: Automatically identifies and filters by genres in your query
- **Rating Filters**: Finds highly-rated books when you ask for "popular" or "best" books
- **Flexible Results**: Ask for specific numbers of recommendations (e.g., "top 5 books")
- **Collection Statistics**: View insights about your book dataset
- **Caching System**: Saves processed embeddings for faster subsequent runs
- **Progress Tracking**: Visual feedback during embedding generation

## 🛠️ Technology Stack

- **Python 3.7+**
- **Google Gemini AI** - Text embedding generation
- **Pandas & NumPy** - Data processing and numerical computations
- **Scikit-learn** - Cosine similarity calculations
- **Requests** - API communication
- **python-dotenv** - Environment variable management

## 📋 Prerequisites

- Python 3.7 or higher
- Google Cloud account with Gemini API access
- Books dataset in CSV format
- API key for Google Gemini

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ai-book-recommender.git
   cd ai-book-recommender
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   
   Create a `.env` file in the root directory:
   ```env
   GOOGLE_API_KEY=your_gemini_api_key_here
   ```

4. **Prepare your dataset**
   
   Place your `books_dataset.csv` file in the root directory with columns:
   - `title` or `Book Name`
   - `author` or `Author Name`
   - `ranking` or `Rating`
   - `genre` or `Genre`
   - `description` or `Description`
   - `release_date` or `Date`
   - `page_numbers` or `Pages`

5. **Run the application**
   ```bash
   python book_recommender.py
   ```


## 🔒 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GOOGLE_API_KEY` | Your Google Gemini API key | Yes |


## 🎯 Key Functionality

### Intelligent Query Processing
- Extracts number of desired recommendations
- Detects genre preferences automatically
- Identifies rating requirements
- Handles multiple preference combinations

### Embedding Management
- Generates comprehensive book descriptions for embedding
- Implements retry logic for API reliability
- Caches embeddings for performance
- Progress tracking during generation

### Recommendation Engine
- Uses semantic similarity for matching
- Applies multiple filtering layers
- Ranks results by relevance
- Provides detailed book information

