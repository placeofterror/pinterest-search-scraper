# Pinterest Search Scraper

[![Apify Actor](https://img.shields.io/badge/Apify-Actor-blue)](https://apify.com/devcake/pinterest-search-scraper)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.10+-blue)](https://www.python.org/)
[![Data Extraction](https://img.shields.io/badge/purpose-data--extraction-orange)](#)

**Search Pinterest by keywords and extract pins with 40+ data fields per pin.** Extract images, saves, engagement metrics, pinner details, board information, product pins with pricing. Perfect for SEO research, trend analysis, content inspiration, and competitive monitoring.

---

## What is Pinterest Search Scraper?

**Pinterest Search Scraper** is a specialized tool for extracting **Pinterest search results by keyword**. Simply provide search queries, and retrieve pins including images, descriptions, engagement metrics, creator information, and product data when available. This tool handles any search query, from broad terms to niche keywords.

## Why Use Pinterest Search Scraper?

### Business Use Cases:
- **SEO Research** - Find trending keywords and content in your niche
- **Trend Analysis** - Track popular pins and topics over time
- **Content Planning** - Discover inspiration for your content calendar
- **Competitor Monitoring** - See what's performing in your market
- **Keyword Research** - Identify high-engagement search terms
- **Product Discovery** - Find trending products with pricing info

## How to Search Pinterest

1. **Open the [Pinterest Search Scraper on Apify](https://apify.com/devcake/pinterest-search-scraper)**
2. **Add search queries** (e.g., "minimalist home office", "sustainable fashion")
3. **Set max results** (up to 250 per query, default: 25)
4. **Enable comments** (optional) - Fetch comments for each pin
5. **Enable proxy** (recommended) - Use Apify Proxy for reliability
6. **Click "Start"** and download your data

**Pro Tip**: Use multiple queries to compare trends across different keywords or niches.

## Features

- **Search by Keyword** - Extract pins from any search query
- **All Image Sizes** - Get every resolution (236x, 474x, 564x, 736x, orig)
- **Engagement Metrics** - Saves, likes, comments, repins, shares
- **Creator Details** - Pinner username, full name, avatar, follower count
- **Board Information** - Board name, URL, pin count, owner
- **Product Pin Detection** - Identify pins with pricing, stock status
- **Comments with Replies** - Optional: Extract user feedback and nested replies
- **No Login Required** - Works without cookies
- **Proxy Support** - Built-in Apify Proxy integration

## Pricing

**Pay per use** — $4 per 1,000 results

No subscriptions, no commitments, no hidden fees. Control your spending with the Maximum Cost Per Run option.

## Input

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `searchQueries` | array | ✅ Yes | Search terms to find pins |
| `maxResults` | integer | No | Max pins per query (1-250, default: 25) |
| `includeComments` | boolean | No | Fetch comments for each pin |
| `maxComments` | integer | No | Max comments per pin (1-100, default: 10) |
| `proxyConfig` | object | No | Proxy configuration (recommended) |
| `maxTotalChargeUsd` | number | No | Spending limit per run (default: $10) |

### Search URL Formats

```
https://www.pinterest.com/search/pins/?q=keyword
https://www.pinterest.com/search/pins/?q=keyword&rs=hub_page
```

## Output Example

```json
{
  "id": "123456789",
  "url": "https://www.pinterest.com/pin/123456789/",
  "title": "Minimalist Home Office Setup",
  "images": {
    "236x": {"url": "https://i.pinimg.com/236x/..."},
    "474x": {"url": "https://i.pinimg.com/474x/..."}
  },
  "saves": 1523,
  "pinner": {
    "username": "designlover",
    "follower_count": 12500
  },
  "board": {
    "name": "Office Inspiration",
    "pin_count": 245
  },
  "is_product_pin": false
}
```

## Related Actors

| Actor | Description | Pricing |
|-------|-------------|---------|
| [Pinterest Pin Scraper](https://github.com/devcake/pinterest-pin-scraper) | Scrape individual pins with product data | $4 per 1,000 pins |
| [Pinterest Profile Scraper](https://github.com/devcake/pinterest-profile-scraper) | Extract user profiles with emails | $4 per 1,000 profiles |
| [Pinterest Board Scraper](https://github.com/devcake/pinterest-board-scraper) | Download complete boards | $4 per 1,000 pins |

## FAQ

### Do I need Pinterest login credentials?
No! This scraper works without login for all public search results.

### How many results can I get per query?
Up to 250 pins per search query. For larger datasets, use multiple runs with different keyword variations.

### Can I search for specific types of pins?
Yes. Include keywords like "product", "buy", "price" to find product pins, or use Pinterest's advanced search filters manually.

### Does this include Pinterest's "More ideas" section?
Yes, the API-based approach captures results from the main search feed.

### Are comments included?
Yes! Enable `includeComments: true` to fetch comments with nested replies for each pin.

## Get it on Apify

[![Run on Apify](https://img.shields.io/badge/Run_on-Apify-informational?style=for-the-badge&logo=apify)](https://apify.com/devcake/pinterest-search-scraper)

**Start searching Pinterest in minutes!**

---

## Also by @devcake

Check out my other scraping tools:

### E-Commerce Suite
- [AlternativeTo Data Scraper](https://github.com/devcake/alternativeto-data-scraper) - Extract software alternatives with license filters
- [Alibaba Products Scraper](https://github.com/devcake/alibaba-products-scraper) - Find profitable products with low MOQ
- [Alibaba Supplier Scraper](https://github.com/devcake/alibaba-supplier-scraper) - Find verified suppliers & manufacturers
- [GlobalSources Products Scraper](https://github.com/devcake/globalsources-products-scraper) - Source from 10M+ verified suppliers
- [GlobalSources Supplier Scraper](https://github.com/devcake/globalsources-supplier-scraper) - 6-level verification data

---

**License**: MIT | **Author**: [@devcake](https://apify.com/u/devcake)

[![GitHub stars](https://img.shields.io/github/stars/devcake/pinterest-search-scraper?style=social)](https://github.com/devcake/pinterest-search-scraper)
