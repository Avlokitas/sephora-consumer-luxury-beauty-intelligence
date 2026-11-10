# Dataset Documentation

## Dataset Source

**Dataset:** Sephora Products and Skincare Reviews  
**Platform:** Kaggle  
**File used:** `product_info.csv`  
**Source:** [Sephora Products and Skincare Reviews – Kaggle](https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews)

This project uses the product catalogue file (`product_info.csv`) from the dataset. The analysis focuses on product-level information rather than individual customer review text.

## Dataset Overview

The dataset contains **8,494 product records** and **27 original columns**, covering product attributes, brand information, customer engagement, ratings, pricing and product availability.

The dataset includes information from **304 brands** across Sephora's product catalogue.

## Key Variables

| Variable | Description |
|---|---|
| `product_id` | Unique product identifier |
| `product_name` | Name of the product |
| `brand_name` | Product brand |
| `loves_count` | Number of users who loved the product |
| `rating` | Average customer rating |
| `reviews` | Number of customer reviews |
| `price_usd` | Product price in USD |
| `value_price_usd` | Product value price, where available |
| `sale_price_usd` | Discounted price, where available |
| `primary_category` | Main product category |
| `secondary_category` | Secondary product category |
| `tertiary_category` | Detailed product category |
| `ingredients` | Product ingredient information |
| `highlights` | Product highlights and features |
| `limited_edition` | Indicates whether a product is limited edition |
| `new` | Indicates whether a product is marked as new |
| `online_only` | Indicates whether a product is available online only |
| `out_of_stock` | Indicates whether a product is marked out of stock |
| `sephora_exclusive` | Indicates whether a product is a Sephora exclusive |

The dataset also contains product variations, sizes, descriptions, child product counts and related pricing fields.

## Data Preparation

The original dataset was cleaned and prepared for exploratory analysis. The workflow included:

- Checking missing values and duplicate records.
- Reviewing data types and product attributes.
- Examining pricing, ratings and engagement distributions.
- Creating derived variables for product segmentation and pricing analysis.
- Preparing an analysis-ready dataset for Tableau visualisation.

## Analytical Scope

The project uses catalogue-level metrics to examine:

- Product engagement through loves and review counts.
- Reported customer satisfaction through product ratings.
- Brand and category-level winner representation.
- Product pricing and relative price positioning.
- Product attributes such as exclusivity, newness and availability.

**Important:** `loves_count` and `reviews` are engagement proxies, not direct measures of purchases or revenue. Products with unavailable ratings should not automatically be interpreted as low-satisfaction products.

## Data Access

The original dataset is available through Kaggle. Please download `product_info.csv` from the source linked above and place it in the appropriate data directory when reproducing the analysis.

The raw dataset is not included in this repository.
