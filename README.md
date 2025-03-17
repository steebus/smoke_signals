# Smoke Signals in Pop Culture

## Analysing Smoking References in Music and Its Social Impact via NLP

This project examines the relationship between smoking references in popular music and smoking prevalence in Australia over seven decades (1945-2023). Using web scraping, natural language processing, and machine learning techniques, I explore whether popular culture reflected in music lyrics correlates with public health trends.

## Key Features

- **Data Collection Pipeline**: Custom-built web scrapers to gather music popularity data from multiple sources:
     - Kent Music Report (1955-1987) via Wikipedia
     - ARIA Charts (1988-2023) via official website
     - Triple J Hottest 100 (1993-2023) via Wikipedia

- **Lyrics Extraction System**: Multi-tiered web scraping approach for gathering song lyrics from Genius.com:
    - Direct URL construction
    - API search functionality
    - Advanced text cleaning for improved matching

- **NLP Processing**: Comprehensive text analysis pipeline including:
    - Text cleaning and normalization
    - Stopword removal with custom music-specific additions
    - Keyword identification and counting
    - TF-IDF (Term Frequency-Inverse Document Frequency) analysis

- **Smoking Reference Lexicon**: Custom-built lexicon of smoking-related terms, expanded using Word2Vec embeddings to capture semantic relationships

- **Time Series Analysis**: Aggregation of smoking references by year with various metrics:
    - Total references
    - References per song
    - 10-year rolling averages
    - Comparative analysis with smoking prevalence data

- **Machine Learning Models**:
    - Linear Regression (baseline model)
    - Support Vector Regression with hyperparameter tuning
    - Feature scaling and preprocessing
    - Performance evaluation with R² scores of up to 0.893

## Technical Stack

- **Python**: Primary programming language
- **Data Manipulation**: Pandas, NumPy
- **Web Scraping**: BeautifulSoup, Requests
- **Natural Language Processing**: NLTK, Gensim, Word2Vec
- **Machine Learning**: Scikit-learn
- **Data Visualization**: Matplotlib, Seaborn
- **Interpolation**: SciPy (PchipInterpolator)

## Key Findings

- Strong correlation between smoking references in music and smoking prevalence in Australia
- Non-linear relationship better captured by SVR model (R² = 0.893) than linear regression (R² = 0.798)
- Identified top songs with highest smoking references, with "Smoke It" by The Dandy Warhols and "(Let's Go) Smoke Some Pot" by Dash Rip Rock leading the list
- "Smoke" is the most frequently used smoking-related term in popular music

## Project Structure

- `data/`: Raw and processed datasets
- `README.md`: Project documentation

## Future Work

- Expand analysis to include other countries and cultural contexts
- Incorporate sentiment analysis to understand the portrayal of smoking
- Investigate causal relationships through more advanced modelling
- Apply word sense disambiguation to reduce false positives
- Integrate additional media sources (films, TV shows) for a comprehensive analysis

## Acknowledgements

- Australian Institute of Health and Welfare for smoking prevalence data
- Cancer Council Victoria for historical smoking statistics
- Wikipedia and ARIA for music chart information
- Genius.com for lyrics data

## License

This project is licensed under the MIT License - see the LICENSE file for details.