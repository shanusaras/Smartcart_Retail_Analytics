# Web Scraping Module

## Purpose
This module demonstrates web scraping capabilities for e-commerce data collection. It serves two main purposes in this project:

1. **Educational Demonstration**: Shows how to collect e-commerce data programmatically
2. **Alternative Data Source**: Provides a method to gather additional product/pricing data

## ⚠️ Important Note
- The main analysis in this project uses the Kaggle dataset (`ecomm_invoice_transaction.parquet`)
- This web scraping component is included to demonstrate data collection skills
- It's not required for the core analysis but shows the complete data pipeline

## Components

### 1. Main Scraping Scripts
- `ecommerce_script.py`: Primary script using Selenium for dynamic content
- `ecommerce_script_old.py`: Deprecated version (kept for reference)
- `slider_solver.py` & `slider_solver_new.py`: Handle CAPTCHA/slider verification

### 2. Scrapy Project (`ecommerce_scraper/`)
A structured approach to web scraping with:
- `spiders/`: Contains the actual scraping logic
- `items.py`: Defines data structure for scraped items
- `pipelines.py`: Processes and validates scraped data
- `middlewares.py`: Handles requests/responses
- `settings.py`: Configuration for the scraping project

## Data Collection Disclaimer

This module was developed for educational purposes only. Key considerations:

1. **Legal Compliance**
   - Users must comply with target websites' Terms of Service
   - Always check `robots.txt` before scraping
   - Respect `Crawl-delay` and other directives

2. **Ethical Scraping**
   - Rate limiting implemented (1s delay between requests)
   - No personal/sensitive data collected
   - Proper attribution given to data sources

## Setup & Usage

### Prerequisites
```bash
pip install scrapy selenium pillow
```

### Running the Scraper
1. Configure target URLs in the script
2. Run the main script:
   ```bash
   python ecommerce_script.py
   ```
   Or use Scrapy directly:
   ```bash
   cd ecommerce_scraper
   scrapy crawl your_spider_name
   ```

## Integration with Main Project
- The scraped data can be processed and merged with the main dataset
- See `notebooks/ecomm_eda.ipynb` for data processing examples

## Note
This code is provided as-is for educational purposes. Always obtain proper authorization before scraping any website.
