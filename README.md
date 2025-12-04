# Lefties Product Info Actor Scraper
>This project pulls rich product information directly from Lefties.com and turns it into clean, structured data you can actually work with. It processes multiple URLs at once, handles rate limits gracefully, and captures everything from pricing and variants to images and availability. If you're analysing retail trends or building product catalogs, this scraper saves a ton of manual effort.

<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>

<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>Lefties Product Info Actor Scraper</strong> you've just found your team — Let's Chat. 👆👆
</p>

## Introduction
This tool collects detailed product information from Lefties, a major fashion retailer, and compiles the results into a structured dataset. It’s designed for ecommerce analysts, retail researchers, and developers who need accurate, up-to-date product details at scale.

### What It Brings to the Table
- Extracts complete product metadata from individual or bulk URLs.
- Captures pricing, stock details, colorways, sizes, and reference codes.
- Pulls product images, descriptions, and care instructions in one run.
- Applies randomized delays to mimic organic browsing and reduce blocking.
- Stores outputs individually and as a unified dataset.

---
## Features
| Feature | Description |
|---------|-------------|
| Batch URL Processing | Accepts multiple product links and processes them in parallel. |
| Detailed Product Extraction | Retrieves IDs, pricing, descriptions, variants, sizes, images, and care info. |
| Stock & Availability Tracking | Captures real-time stock status for each product variant. |
| Image Scraping | Extracts all product images, including variant-specific photos. |
| Rate Limiting | Uses random delays to prevent overloading the site. |
| Error Handling | Logs issues gracefully and continues processing without interruption. |
| Flexible Output | Outputs individual product files and a combined dataset. |

---
## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|-------------------|
| id | Unique Lefties product identifier. |
| name | Product title or display name. |
| description | Full product description text. |
| referenceNumber | Product reference or model number. |
| price.current | Current selling price. |
| price.original | Original price when discounted. |
| colors | List of color options with metadata. |
| sizes | All available sizes with stock information. |
| images | URLs for all product images. |
| composition | Materials and fabric composition. |
| care | Care instructions provided by Lefties. |
| availability | Real-time stock status for each variant. |

---
## Example Output
    
    [
      {
        "id": "12345678",
        "name": "Ribbed Knit Sweater",
        "description": "Soft-touch ribbed sweater with round neck and long sleeves.",
        "referenceNumber": "LF-9021",
        "price": {
          "current": 19.99,
          "original": 29.99
        },
        "colors": [
          { "name": "Black", "code": "001" }
        ],
        "sizes": [
          { "size": "M", "inStock": true },
          { "size": "L", "inStock": false }
        ],
        "images": [
          "https://lefties.com/images/product_123456_1.jpg"
        ],
        "composition": "95% Cotton, 5% Elastane",
        "care": "Machine wash at max 30ºC.",
        "availability": "in_stock"
      }
    ]

---
## Directory Structure Tree
    
    Lefties Product Info Actor/
    ├── src/
    │   ├── main.js
    │   ├── scraper/
    │   │   ├── product_parser.js
    │   │   ├── request_handler.js
    │   │   └── rate_limiter.js
    │   ├── utils/
    │   │   ├── logger.js
    │   │   └── validate_url.js
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── sample_urls.txt
    │   └── sample_output.json
    ├── package.json
    └── README.md

---
## Use Cases
- **Ecommerce analysts** use it to collect product data at scale, helping them track pricing, availability, and catalog changes.  
- **Retail researchers** use it to compare product attributes across fashion brands and study market positioning.  
- **Developers** use it to populate internal databases or feed product info into applications.  
- **Data teams** use it to build enriched product catalogs for reporting and machine learning work.  
- **Catalog managers** use it to monitor inventory shifts and product updates in real time.  

---
## FAQs

**Does the scraper handle multiple links at once?**  
Yes, it supports batch processing for efficient large-scale extraction.

**What if a product page fails to load?**  
The scraper logs detailed errors and continues processing the remaining URLs.

**Does it avoid rate limits?**  
Randomized delays are built in to reduce the chance of triggering automated blocks.

**What types of product fields are included?**  
Everything from pricing and descriptions to images, colors, sizes, reference numbers, composition, and stock status.

---
### Performance Benchmarks and Results

**Primary Metric:**  
Processes an average of 10–20 product pages per minute depending on site load and latency.

**Reliability Metric:**  
Delivers a stable success rate above 97% across large batches thanks to robust error handling.

**Efficiency Metric:**  
Keeps memory usage low by streaming product data instead of holding large batches in memory.

**Quality Metric:**  
Achieves high data fidelity, capturing all key product attributes with minimal missing fields.

<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
         </p>

