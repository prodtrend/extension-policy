# ProdTrend -- Amazon Product Scraper Chrome Extension

ProdTrend is a Chrome extension designed to scrape Amazon search results
and product detail pages.\
It helps in collecting product data for analysis, research, and
competitive tracking.

------------------------------------------------------------------------

## 📌 Features

### ✅ Scrape Search Page

Extracts product metadata such as: - Title\
- Price\
- Ratings\
- Reviews\
- ASIN\
- Product link\
- Image

### ✅ Scrape Product Detail Page

Captures detailed information including: - Bullet points\
- Variations (size/color/style)\
- Technical details\
- Description\
- Additional attributes provided by Amazon

### ✅ Scrape & Save / Analyze All

**Scrape & Save** -- Collect and store product details\
**Analyze All** -- Scrape all visible products in bulk\
**Un‑Analyze Products** -- Reset previously scraped data

------------------------------------------------------------------------

## 🛠 How It Works

ProdTrend injects a `content_script` into Amazon pages.\
It listens for product data, scrapes DOM elements, and stores results in
a global storage container:

-   `prodtrend_extension_global_storage`
-   Shadow DOM support included
-   jQuery + Bootstrap + Custom JS binding

The extension processes: - Product top section\
- Variation selectors\
- Drop-down menus\
- ShadowRoot-based product sections

------------------------------------------------------------------------

## 📂 Project Structure

    ProdTrend/
    │
    ├── manifest.json
    ├── js/
    │   ├── content.js
    │   ├── product_detail.js
    │   ├── search_page.js
    │   └── jquery-3.6.3.min.js
    │
    ├── css/
    │   └── bootstrap.min.css
    │
    └── icons/
        ├── 16.png
        ├── 48.png
        └── 128.png

------------------------------------------------------------------------

## ⚙️ Installation

1.  Open **chrome://extensions/**\
2.  Enable **Developer mode**\
3.  Click **Load Unpacked**\
4.  Select the extension folder\
5.  Visit Amazon and start scraping!

------------------------------------------------------------------------

## 🧪 Limitations / Notes

-   Amazon UI varies between devices; some selectors may break over
    time.\
-   Always validate scraped data manually.\
-   Avoid excessive scraping to comply with Amazon policies.

------------------------------------------------------------------------

## 📜 License

MIT License

------------------------------------------------------------------------

## 🤝 Contributing

Pull requests are welcome!\
For major changes, open an issue to discuss improvements.

------------------------------------------------------------------------

## 📧 Support

For fixes, suggestions, or help integrating this with your workflow,
feel free to reach out.
