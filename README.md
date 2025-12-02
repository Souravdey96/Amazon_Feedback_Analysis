# Amazon Product Feedback Analysis — Summary

This project analyzes ~3,077 Amazon product reviews to understand rating patterns, sentiment, and factors that drive review helpfulness.

## Data Collection & Cleaning
- Dataset includes 13 fields (rating, text, recommendation flag, brand, categories, helpful votes, etc.).  
- Normalized column names and parsed review dates (limited to ~276 entries).  
- Filled missing `do_recommend` values with "Unknown" and removed rows without review text.  
- Engineered features:
  - **Review length** (word count)  
  - **Sentiment polarity** (–1 to +1)  
  - **Helpfulness ratio** (helpful votes / review length)

## Data Analysis
- **Ratings:** ~70% of reviews are 4–5 stars; ~15% are 1–2 stars.  
- **Recommendation trends:** Positive ratings strongly correlate with “doRecommend = True.”  
- **Brand insights:** Some brands score >0.6 sentiment on average; weaker brands score ~0.2.  
- **Category insights:** Electronics show high sentiment variability; Books remain more consistent.  
- **Text insights:**  
  - Positive terms: “quality,” “easy,” “recommend”  
  - Negative terms: “defective,” “return,” “battery”  
  - Longer reviews (~200+ words) attract ~2× more helpful votes.

## Visualizations
- Rating & recommendation bar charts  
- Sentiment heatmap for top brands and categories  
- Word clouds for positive vs negative reviews  
- Scatter of review length vs helpful votes  
- Box plots for helpfulness ratio by rating

## Key Findings
- Negative reviews offer deeper product insights despite being fewer.  
- Detailed “pros & cons”–style reviews produce the highest helpfulness engagement.  
- Improvement opportunities appear around defect-related issues and low-sentiment brands.  
- High-performing brands can enhance marketing by highlighting features that drive strong sentiment.

