# NLP Article Analyzer with GUI for Google Colab

A comprehensive Natural Language Processing (NLP) tool designed for analyzing newspaper articles using various NLP techniques. This interactive tool features a user-friendly GUI interface and provides detailed analysis with visualizations.

## 🚀 Features

### Core NLP Techniques
- **Tokenization**: Break text into sentences and words
- **Stopword Removal**: Filter out common words for better analysis
- **Named Entity Recognition (NER)**: Identify people, places, organizations, and other entities
- **Part-of-Speech (POS) Tagging**: Analyze grammatical structure
- **Sentiment Analysis**: Determine emotional tone and objectivity

### Visualizations
- Word clouds for visual text representation
- POS distribution charts (bar and pie charts)
- Named entity type distribution
- Sentiment analysis graphs
- Statistical summaries

## 📋 Requirements

### Python Libraries
- `nltk` - Natural Language Toolkit
- `spacy` - Advanced NLP library
- `textblob` - Simplified text processing
- `pandas` - Data manipulation
- `matplotlib` - Plotting library
- `seaborn` - Statistical data visualization
- `wordcloud` - Word cloud generation
- `ipywidgets` - Interactive widgets for Jupyter

### NLTK Data Downloads
The following NLTK datasets are automatically downloaded:
- `punkt` - Sentence tokenization
- `punkt_tab` - Additional tokenization resources
- `stopwords` - Common stopwords
- `pos_tag` - Part-of-speech tagging
- `vader_lexicon` - Sentiment analysis
- `averaged_perceptron_tagger` - POS tagger

### spaCy Model
- `en_core_web_sm` - English language model

## 🔧 Installation

### For Google Colab (Recommended)
```python
# Run this cell first to install all required packages
!pip install nltk spacy textblob ipywidgets matplotlib seaborn wordcloud
!python -m spacy download en_core_web_sm
```

### For Local Environment
```bash
pip install nltk spacy textblob ipywidgets matplotlib seaborn wordcloud
python -m spacy download en_core_web_sm
```

## 🎯 Usage

### Quick Start
1. **Copy the code** into a Google Colab notebook
2. **Run the installation cell** first
3. **Execute the main code** to launch the GUI
4. **Paste your article** (150-300 words recommended) into the text area
5. **Click "Analyze Article"** to see comprehensive NLP analysis

### Sample Analysis Output
The tool provides detailed analysis including:
- Text statistics (word count, sentence count)
- Tokenization results
- Stopword removal statistics
- Named entities with classifications
- POS tag distributions
- Sentiment scores with interpretations
- Visual representations (word clouds, charts)

## 📊 Analysis Components

### 1. Tokenization
- Splits text into sentences and individual words
- Cleans text by removing punctuation and converting to lowercase
- Provides word and sentence counts

### 2. Stopword Removal
- Filters out common English words (the, and, is, etc.)
- Shows before/after comparison
- Improves focus on meaningful content words

### 3. Named Entity Recognition (NER)
- Identifies and classifies entities:
  - **PERSON**: Names of people
  - **ORG**: Organizations, companies
  - **GPE**: Countries, cities, states
  - **DATE**: Dates and time periods
  - **MONEY**: Monetary values
  - **And more...**

### 4. Part-of-Speech Tagging
- Tags each word with grammatical role:
  - **NOUN**: People, places, things
  - **VERB**: Actions, states
  - **ADJ**: Descriptive words
  - **ADV**: Modifiers
  - **And more...**

### 5. Sentiment Analysis
- **Polarity**: Measures positive/negative sentiment (-1 to +1)
- **Subjectivity**: Measures objectivity/subjectivity (0 to 1)
- **Classification**: Positive, Negative, or Neutral

## 💡 Example Use Cases

- **Journalism Analysis**: Analyze news articles for bias and entity coverage
- **Content Research**: Extract key entities and topics from articles
- **Educational Tool**: Learn NLP concepts with hands-on analysis
- **Text Mining**: Process large collections of news articles
- **Sentiment Monitoring**: Track sentiment trends in news coverage

## 🎨 Sample Article

The tool comes with a pre-loaded sample article about climate change to demonstrate all features. You can replace it with your own content for analysis.

## 📈 Output Interpretation

### Sentiment Scores
- **Polarity > 0.1**: Positive sentiment
- **Polarity < -0.1**: Negative sentiment  
- **-0.1 ≤ Polarity ≤ 0.1**: Neutral sentiment
- **Subjectivity > 0.5**: Subjective/opinionated
- **Subjectivity ≤ 0.5**: Objective/factual

### Entity Types
Common entity labels and their meanings:
- **PERSON**: Individual people
- **ORG**: Organizations, companies, agencies
- **GPE**: Geopolitical entities (countries, cities)
- **DATE**: Absolute or relative dates
- **TIME**: Times smaller than a day
- **PERCENT**: Percentage values
- **MONEY**: Monetary values
- **QUANTITY**: Measurements, counts

## 🔍 Technical Details

### NLPAnalyzer Class Methods
- `tokenize_text()`: Sentence and word tokenization
- `remove_stopwords()`: Stopword filtering
- `named_entity_recognition()`: Entity extraction
- `pos_tagging()`: Grammatical analysis
- `sentiment_analysis()`: Sentiment scoring
- `generate_wordcloud()`: Visual word representation
- `visualize_pos_distribution()`: POS charts
- `visualize_entities()`: Entity distribution charts

### GUI Components
- Interactive text area for article input
- Analysis button with success styling
- Real-time output display with visualizations
- Comprehensive analysis summaries

## 🚨 Important Notes

- **Minimum Text Length**: Articles should be at least 50 words for meaningful analysis
- **Optimal Length**: 150-300 words recommended for best results
- **Google Colab**: Designed specifically for Colab environment
- **Internet Required**: Initial setup downloads language models
- **Processing Time**: Analysis may take 10-30 seconds depending on article length

## 🤝 Contributing

Feel free to enhance this tool by:
- Adding more NLP techniques
- Improving visualizations
- Supporting additional languages
- Optimizing performance
- Adding export features

## 📄 License

This project is open source and available for educational and research purposes.

## 🆘 Troubleshooting

### Common Issues
1. **Import Errors**: Ensure all packages are installed via the installation cell
2. **spaCy Model Missing**: Run `!python -m spacy download en_core_web_sm`
3. **NLTK Data Missing**: The code automatically downloads required NLTK data
4. **Empty Analysis**: Ensure article has at least 50 words
5. **Widget Display Issues**: Restart runtime and run cells in order

### Support
For issues or questions, check that all installation steps are completed and the notebook runtime is properly configured for Google Colab.

---

**Happy Analyzing! 🎉**
