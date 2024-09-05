# Personalized Nutrient Recommendations Using Knowledge Graphs

## Abstract

This study explores the efficiency and effectiveness of knowledge graphs in providing personalized nutrient recommendations by utilizing dynamic, interconnected data structures that integrate diverse sources of information. Through the application of logistic regression, our research demonstrates that knowledge graphs offer a compelling alternative to traditional content-based methods. While not surpassing them in all aspects, the knowledge graph-based approach can provide recommendations that are not only accurate but also richly diverse, improving user satisfaction. Twelve participants in the evaluation appreciated the approach’s ability to offer a wide array of relevant ingredients and recipes tailored to their nutritional preferences. This capability allowed users to receive healthy suggestions aligned with their individual nutritional needs and tastes. Future efforts should focus on automating the knowledge graph-building process, broadening the diversity of suggested ingredients and recipes, and integrating with online grocery services to enhance practicality.

## Introduction

Personalized nutrition aims to optimize health by offering tailored recommendations that meet individual needs. This approach integrates diverse data types, including nutrition information, personal profiles, lifestyles, and dietary habits. Key challenges include integrating diverse data sources, accurately modeling health profiles, and adapting to dynamic health information. Our research addresses these challenges by leveraging knowledge graphs to enhance personalization, relevance, and diversity in nutrient recommendations.

## Methodology

1. **Data Collection and Preparation:** Gather and prepare data for analysis.
2. **Exploratory Data Analysis:** Investigate data to identify patterns and anomalies.
3. **Feature Engineering:** Create relevant features from the data.
4. **Model Development:** Develop and train various machine learning models.
5. **Model Evaluation:** Assess model performance using various metrics.
6. **External Validation:** Test the final model on new data to ensure robustness.

## Implementation Details

- **Neo4j:** Used for constructing and managing the knowledge graph.
- **Data Integration:** Mapping user profile data to the knowledge graph, including ingredients, recipes, and diet types.
- **Predictive Modeling:** Utilizing logistic regression and various machine learning algorithms to predict user preferences.

### Data Preparation

- Node embeddings were generated using the Fast Random Projection algorithm.
- Enhanced node embeddings with the Hadamard transform.
- Data was split into training, validation, and testing sets.

### Model Training and Evaluation

- Logistic Regression was used for binary classification to predict user preferences.
- Evaluated model performance with AUCPR and OUT_OF_BAG_ERROR.

### Recipe Recommendation Algorithm

1. Retrieve user preferences and predicted liked ingredients.
2. Filter recipes based on dietary restrictions and ingredient preferences.
3. Rank recipes by the number of matched liked ingredients.

## Results

The knowledge graph-based approach successfully provided personalized, contextually relevant recommendations and improved user satisfaction compared to traditional methods.

## Future Work

- Automate the knowledge graph-building process.
- Increase diversity in suggested ingredients and recipes.
- Integrate with online grocery services for enhanced practicality.
