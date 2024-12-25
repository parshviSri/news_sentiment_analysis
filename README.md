# Financial News Sentiment Analysis

This repository demonstrates how to perform web scraping and sentiment analysis on financial news data. The project uses Python to extract news headlines from the Financial Express website and analyze their sentiment using natural language processing techniques.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Setup and Installation](#setup-and-installation)
5. [Usage](#usage)
6. [File Structure](#file-structure)
7. [Contributing](#contributing)
8. [License](#license)

---

## Introduction

Market sentiment analysis can provide insights into trends and public opinion, helping investors and analysts make data-driven decisions. This project automates the collection of financial news and applies sentiment analysis to identify positive, neutral, or negative sentiment in headlines.

---

## Features

- **Web Scraping:** Extracts news headlines and links from the Financial Express website using Selenium.
- **Data Cleaning:** Cleans and preprocesses the text to remove noise and prepare it for analysis.
- **Sentiment Analysis:** Uses the TextBlob library to calculate sentiment polarity for each headline.
- **Visualization:** Visualizes sentiment distribution using histograms.
- **Automation:** Modular functions for reusability and scalability.

---

## Technologies Used

- **Python**
  - Libraries: Selenium, pandas, TextBlob, matplotlib, re
- **Selenium WebDriver** for browser automation
- **TextBlob** for natural language processing
- **Matplotlib** for data visualization

---

## Setup and Installation

### Prerequisites
1. Python 3.x installed on your system.
2. Google Chrome and [ChromeDriver](https://chromedriver.chromium.org/downloads) installed.

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/financial-news-sentiment-analysis.git
   cd financial-news-sentiment-analysis
   ```

2. Install required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up ChromeDriver:
   - Download the ChromeDriver that matches your Chrome browser version.
   - Place it in a directory accessible by the project.

4. Update the `driver_path` in the code to point to your ChromeDriver:
   ```python
   driver = webdriver.Chrome(executable_path="path/to/chromedriver")
   ```

---

## Usage

### 1. Run the Script
Run the main script to scrape financial news and perform sentiment analysis:
```bash
python sentiment_analysis.py
```

### 2. Output
- A DataFrame containing news headlines, their corresponding sentiment scores, and cleaned versions of the headlines.
- A histogram visualizing sentiment polarity distribution.

### 3. Modify for Your Needs
Customize the URL or scraping logic to analyze data from other websites or sources.

---

## File Structure

```
financial-news-sentiment-analysis/
├── README.md                # Project overview and instructions
├── sentiment_analysis.py    # Main script for web scraping and sentiment analysis
├── requirements.txt         # Python library dependencies
└── results/                 # Directory for output data and visualizations
```

---

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add a new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

