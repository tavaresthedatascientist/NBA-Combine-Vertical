## NBA Draft Combine: Predictors of Vertical Jump Performance 

## Overview: 
This project analyzes how a basketball player's physical attributes influence their max vertical jump at the NBA Draft Combine. 
Using combine measurement data from 2009-2017, I applied correlation analysis and multiple linear regression to identify which physical factors best predict a player's leaping ability. 
Results suggest that body composition is a stronger predictor of explosiveness rather than height or weight alone. 


## Research Question:
Which physical attributes (height, weight, body fat %) most strongly predict vertical jump performance at the NBA Draft Combine?

## Dataset
Kaggle NBA Draft Combine dataset
N = 517 players 

## Methods 
- Exploratory scatterplots with regression lines
- Pearson correlation analysis
- Multiple linear regression modeling


## Key Findings 
- R**2 = 0.28 - height, weight, and body fat together explain about 28% of the variation in vertical jump. That suggests that other factors e.g. (athleticism, training regimen, and genetics) play a role in leaping ability.
- All three variables are negatively correlated with vertical jump.

## Regression Coefficients (Multiple Linear Model)
***These represent the expected change in vertical jump (in inches) for a one-unit increase in the predictor, holding variables constant.
- Height: -0.42, indicating for every 1 inch taller a player is, their vertical jump drops by 0.42 inches.
- Weight: +0.01, indicating no independent effect when controlling for height and body fat.
- Body fat: -0.56, indicating the strongest independent association, for every 1% increase in body fat percentage, vertical leap drops by 0.56 inches.
  
***Intercept: 69.23 - this intercept represents the model's predicted vertical jumpwhen all predictors are zero, which isn't practical or meaningful given the context of this dataset. 



## Key Takeaways: 
Controlling for both height and weight, body fat percentage shows the strongest independent negative association with vertical jumping performance, this suggests that body composition may play a more critical role in explosiveness than structural size alone. 

## Visualizations:
![Height vs Vertical Jump](output/height_vs_vertical.png)
![Weight vs Vertical Jump](output/weight_vs_vertical.png)
![Body Fat vs Vertical Jump](output/bodyfat_vs_vertical.png)

## How to Run:
1. Clone the repository
2. Install dependencies: pip install pandas numpy matplotlib seaborn scikit-learn
3. Open notebooks/vertical_jump_analysis.ipynb
4. Run all cells
  
