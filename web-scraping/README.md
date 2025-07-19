# Web Scraping Module

## Data Collection Disclaimer

This web scraping module was developed for educational and portfolio purposes only. The following ethical considerations have been taken into account:

1. **Legal Compliance**
   - This code is shared for educational purposes only
   - Users are responsible for complying with the target website's Terms of Service
   - Always check `robots.txt` before scraping any website

2. **Rate Limiting**
   - Built-in delays between requests (`DOWNLOAD_DELAY = 1`)
   - Respectful scraping practices implemented
   - Concurrent requests are limited

3. **Data Usage**
   - No personal or sensitive information is collected
   - Data is used strictly for analysis and demonstration
   - Dataset is not to be used for commercial purposes

4. **Attribution**
   - Data source should be properly attributed if used in any public work
   - Original website should be credited when sharing analysis results

## Usage for Interview Discussions

When discussing this project in interviews, you can mention:
- The technical implementation of the scraper
- How you handled challenges like dynamic content
- The ethical considerations you implemented
- That the actual data source has been anonymized for privacy

## Setup

1. Install required dependencies:
   ```bash
   pip install scrapy selenium
   ```

2. Configure settings in `ecommerce_scraper/settings.py`

3. Run the scraper:
   ```bash
   scrapy crawl your_spider_name
   ```

## Note
This code is provided as-is for educational purposes. Always obtain proper authorization before scraping any website.
