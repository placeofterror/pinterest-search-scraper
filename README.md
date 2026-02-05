# Pinterest Search Scraper

[![Apify Actor](https://img.shields.io/badge/Apify-Actor-blue)](https://apify.com/devcake/pinterest-search-scraper)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.10+-blue)](https://www.python.org/)
[![Data Extraction](https://img.shields.io/badge/purpose-data--extraction-orange)](#)

**Scrape Pinterest search results with 40+ data fields.** Extract pins, images, prices, engagement metrics, and more from Pinterest search by keyword. Perfect for market research, competitor analysis, and SEO tracking.

---

## What is Pinterest Search Scraper?

**Pinterest Search Scraper** is a powerful data extraction tool that enables you to scrape **Pinterest search results** at scale. Simply enter your search keywords, and extract comprehensive data including pin titles, descriptions, images, prices, engagement metrics, and author profiles. This tool handles Pinterest's dynamic content loading, pagination, and anti-scraping measures automatically.

## Why Use Pinterest Search Scraper?

### Business Use Cases:
- **Market Research**: Discover trending products and content in your niche
- **Competitor Analysis**: Monitor what your competitors are pinning and how users engage
- **SEO Strategy**: Find high-performing keywords and content ideas
- **Content Planning**: Identify viral pin patterns to inform your marketing
- **Product Sourcing**: Find popular products with proven engagement metrics
- **Influencer Discovery**: Locate pinners with high engagement for partnerships

## How to Scrape Pinterest Search Results

1. **Open the [Pinterest Search Scraper on Apify](https://apify.com/devcake/pinterest-search-scraper)**
2. **Enter your search keywords** (e.g., "wedding decoration", "vegan recipes")
3. **Configure options** (max items, proxy settings)
4. **Click "Start"** and wait for extraction
5. **Download data** in JSON, CSV, or Excel formats

**Pro Tip**: Use multiple search runs with related keywords to build comprehensive datasets for trend analysis.

## Features

✅ **40+ Data Fields** - Extract comprehensive pin data including title, description, image URLs, prices, saves, comments, and more

✅ **Automatic Pagination** - Handles infinite scroll and page navigation automatically

✅ **Proxy Rotation** - Built-in proxy support to avoid IP blocks

✅ **Multiple Search Queries** - Process multiple keywords in a single run

✅ **Flexible Output** - Export data in JSON, CSV, Excel, or HTML formats

✅ **Fast & Reliable** - Optimized extraction with minimal resource usage

✅ **Scheduled Runs** - Set up recurring scrapes for continuous monitoring

## Pricing

| Plan | Price | Results |
|------|-------|---------|
| Pay-per-event | **$4.00** | 1,000 pins |
| Monthly | Custom | Unlimited |

**Try it free** with Apify's trial credits!

## Input Example

```json
{
  "searchQueries": ["wedding ideas", "home decor"],
  "maxItems": 100,
  "proxy": {
    "useApifyProxy": true
  }
}
```

## Output Example

```json
{
  "pinId": "123456789",
  "title": "Rustic Wedding Centerpiece Ideas",
  "description": "Beautiful mason jar centerpieces...",
  "imageUrl": "https://i.pinimg.com/...",
  "price": "$24.99",
  "saves": 15234,
  "comments": 342,
  "authorName": "Sarah's Wedding Blog",
  "authorUsername": "@sarahweddings",
  "boardName": "Wedding Inspiration",
  "pinUrl": "https://pinterest.com/pin/123456789"
}
```

## Related Actors

| Actor | Description |
|-------|-------------|
| [Pinterest Board Scraper](https://github.com/Bahm9919/pinterest-board-scraper) | Download complete Pinterest boards |
| [Pinterest Profile Scraper](https://github.com/Bahm9919/pinterest-profile-scraper) | Extract user profiles with emails |
| [Pinterest Pin Scraper](https://github.com/Bahm9919/pinterest-pin-scraper) | Scrape individual pins with product data |

## FAQ

### Is scraping Pinterest legal?
Yes, scraping public data from Pinterest for research and analysis purposes is generally legal. However, always respect Pinterest's Terms of Service and robots.txt. This tool is intended for legitimate business use cases only.

### How can I avoid being blocked?
This tool includes built-in proxy rotation. For large-scale scraping, we recommend using residential proxies and limiting request rates.

### Can I scrape Pinterest without an account?
Yes! This scraper doesn't require a Pinterest account. It extracts publicly available data from search results.

### What data can I extract?
You can extract 40+ fields including: pin ID, title, description, image URLs, price, availability, save count, comment count, author details, board info, and direct pin URLs.

### How do I handle pagination?
The scraper handles pagination automatically. Just set your desired `maxItems` and the tool will paginate until it reaches the limit or exhausts results.

## Get it on Apify

[![Run on Apify](https://img.shields.io/badge/Run_on-Apify-informational?style=for-the-badge&logo=apify)](https://apify.com/devcake/pinterest-search-scraper)

**Start scraping Pinterest search results in minutes!**

---

## Also by @devcake

Check out my other scraping tools:

- [AlternativeTo Data Scraper](https://github.com/Bahm9919/alternativeto-data-scraper)
- [Alibaba Products Scraper](https://github.com/Bahm9919/alibaba-products-scraper)
- [Alibaba Supplier Scraper](https://github.com/Bahm9919/alibaba-supplier-scraper)
- [GlobalSources Products Scraper](https://github.com/Bahm9919/globalsources-products-scraper)

---

**License**: MIT | **Author**: [@devcake](https://apify.com/u/devcake)

[![GitHub stars](https://img.shields.io/github/stars/Bahm9919/pinterest-search-scraper?style=social)](https://github.com/Bahm9919/pinterest-search-scraper)
