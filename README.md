# MediaBias Analyzer

MediaBiasAnalyzer is a Python script that uses OpenAI's API to analyze news articles for political bias. It determines whether an article is left-leaning, right-leaning, or neutral and provides reasoning for its conclusions along with a numerical rating using **"AllSides Media Bias Ratings" methodology (read more here: https://www.allsides.com/media-bias/media-bias-rating-methods). The goal of this project is to promote transparency and awareness of political bias in media.

## Features
- Scrapes text from news articles.
- Analyzes political bias using OpenAI's GPT-based models.
- Provides detailed reasoning for the classification.

## Prerequisites
1. **Python 3.8 or later**
2. **Required Python Libraries**:
   - `openai`
   - `requests`
   - `beautifulsoup4`

To install the required libraries, run:
```bash
pip install openai requests beautifulsoup4
```

3. **OpenAI API Key**:
   - Set up an OpenAI account and generate an API key.
   - Export the API key as an environment variable:
     ```bash
     export OPENAI_API_KEY="your-api-key-here"
     ```

## Usage

1. Clone the repository:
```bash
git clone https://github.com/your-username/mediabias-analyzer.git
cd mediabias-analyzer
```

2. Run the program:
```bash
python main.py
```

3. Input the URL of a news article when prompted.

The program will scrape the article's content and analyze its political bias, returning the result along with the reasoning.

## Example Output
```
Enter the URL of the news article: https://example.com/news-article

--- Bias Analysis ---
The article is left-leaning.
Reasoning: The article emphasizes progressive viewpoints, criticizes conservative policies, and uses language that aligns with left-wing ideology.
```

## Next Steps

### Data Collection and Storage
The next phase of the project involves:
- **Collecting Articles**: Scraping a large number of articles from various news sources.
- **Storing Results**: Creating a database to store the analysis results.
- **Source Analysis**: Aggregating data to determine whether each news source leans left, right, or remains neutral over time.

### Future Enhancements
- Incorporating sentiment analysis to provide deeper insights.
- Visualizing trends in media bias across sources and regions.
- Allowing users to upload articles or input text directly for analysis.
