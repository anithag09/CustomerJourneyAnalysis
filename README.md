# Customer Journey Analysis
This project provides tools to analyze customer journeys using data from user interactions with products. The analysis includes sentiment analysis of customer reviews, product ratings, price sensitivity, and behavior patterns within various product categories. The main goal is to extract meaningful insights into customer behavior and satisfaction trends.

## Features
- Sentiment Analysis: Uses TextBlob to assess sentiment polarity in customer reviews.
- User Behavior Analysis: Identifies user interaction patterns, including rating behavior, price sensitivity, and category preferences.
- Category Analysis: Extracts insights on product categories based on reviews, ratings, and discount impact.
- Journey Factors: Determines key factors that influence customer satisfaction, such as discount usage and price range performance.
- Common Terms Extraction: Uses TF-IDF to identify frequently mentioned terms in positive reviews within each category.

## Data Preprocessing
The data preprocessing pipeline includes:

- Sentiment Calculation: Each customer review is assigned a sentiment score based on polarity.
- Binary Feature Creation: Identifies whether the customer has left a review or rating.
- Price Sensitivity Calculation: A measure of how responsive customers are to discounts.

## Analysis Capabilities
1. User Pattern Analysis
The analyze_user_patterns method aggregates user behavior metrics:
Total interactions with products.
Average and standard deviation of ratings and sentiment.
Price sensitivity and discount preferences.
Preferred product categories.

2. Category Insights
The analyze_category_patterns method evaluates product categories by:
Average rating and review sentiment.
Correlation between discounts and ratings.
Common terms in positive reviews.

3. Journey Factors
The analyze_journey_factors method explores key drivers of customer satisfaction:
The correlation between ratings, sentiment, and pricing.
Review patterns, including review rate and sentiment distribution.
Price impact on customer satisfaction based on discounts and price ranges.

## Dependencies
- pandas
- numpy
- textblob
- scikit-learn

## Installation
To run this project, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/anithag09/CustomerJourneyAnalysis.git
   ```

## Dataset
The project expects the input data to contain the following columns:

- user_id: ID of the user.
- product_id: ID of the product.
- rating: Product rating by the user.
- normalized_review: Preprocessed text of the customer review.
- discount_percentage: Discount applied to the product at the time of purchase.
- actual_price: Final price after the discount.
- category: Category of the product.

## Contributing
Feel free to open issues or contribute by creating pull requests. Any contributions, suggestions, or improvements are welcome.
