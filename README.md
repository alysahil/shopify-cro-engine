# ⚡ Shopify CRO Opportunity Engine

A premium, macOS-inspired single-page web application that performs real-time conversion rate optimization (CRO) audits on public Shopify storefronts.

🔗 **GitHub Repository**: [github.com/alysahil/shopify-cro-engine](https://github.com/alysahil/shopify-cro-engine)

---

## 🎨 Design Philosophy & UI
- **macOS Window Aesthetic**: Clean dark mode with standard macOS window controls, subtle glassmorphic elements, and mesh background gradients.
- **Micro-Animations**: Smooth entry transitions, hover states, and live pulsing status indicators for background API requests.
- **Responsive Layout**: Adapts perfectly to mobile and desktop screens.

---

## ✨ Features

### 1. 📡 Real-Time Public API Integrations
- **Product & Collection Feed**: Fetches real catalog data directly from `[store-url]/products.json` and `[store-url]/collections.json` (no API keys required).
- **Currency Detection**: Queries the store's `/cart.js` endpoint to extract and format values using the store's local currency (e.g., `INR`, `USD`, `GBP`).
- **Google PageSpeed Insights API**: Automatically fetches LCP, FCP, TBT, CLS, Speed Index, and overall Performance Score for mobile devices.
- **Tech Stack Profiling**: Scrapes the homepage via proxy to identify active marketing, chat, loyalty, reviews, payments, and analytics tools.

### 2. 📊 ICE-Scored Opportunity Analysis
Prioritizes recommendations based on the **ICE Framework** (Impact × Confidence ÷ Effort):
- **Image Coverage**: Audits products for multiple images and benchmark standard (4+ photos).
- **Description Quality**: Evaluates character length and copy quality.
- **Pricing & Discounts**: Scans for compare-at price coverage and discounting frequency.
- **Stock Health**: Calculates out-of-stock (OOS) and partial OOS rates.
- **Discoverability**: Analyzes product-to-collection distribution ratios.
- **AOV Lift**: Detects bundle/kit availability.
- **Trust Factors**: Checks for integration of review apps.

### 🧪 3. Structured A/B Experiment Briefs
Generates comprehensive A/B testing briefs for the top 5 ICE-ranked recommendations, outlining:
- Core hypothesis and supporting evidence.
- Split-testing controls and treatments.
- Primary, secondary, and guardrail metrics.
- Recommended test duration and traffic split.

### ⚔️ 4. Competitor Benchmarking
Allows direct comparisons of any two Shopify stores across major catalog metrics, tech stack features, and PageSpeed metrics.

### 💾 5. Data Portability
- **Live Data Preview**: Displays a sample table of the first 6 fetched items to verify data authenticity.
- **JSON Export**: Downloads the generated audit data and scoring logs in a structured JSON schema.

---

## 🚀 How to Run Locally

Since this is a client-side application with zero dependencies, you can run it in seconds:

1. Clone this repository:
   ```bash
   git clone https://github.com/alysahil/shopify-cro-engine.git
   ```
2. Navigate to the folder and open the `index.html` file in any modern web browser:
   - **Double-click** `index.html` in your file manager.
   - Or open via terminal:
     ```powershell
     Start-Process index.html
     ```

---

## 📦 How to Deploy
Because the app is composed entirely of static assets, it can be deployed for free:
- **Vercel**: Import this repository directly or upload the folder on Vercel.
- **Netlify**: Drag and drop the folder into **[Netlify Drop](https://app.netlify.com/drop)**.