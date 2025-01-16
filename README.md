## Lok-MSDS-460-Assignment-1
MSDS 460 | Maddy Lok | 15 January 2025

# Using a Linear Programming Model to Optimize a Personal Diet

## Overview
This project applies **Linear Programming (LP)** to construct a cost-efficient diet that satisfies **U.S. FDA nutritional guidelines** while minimizing cost. The solution leverages **Python and PuLP**, with additional refinements to **increase variety** and **improve practicality**.

## Goal
- **Minimize** the total weekly cost of food while meeting the FDA recommended nutrient intake.
- **Seven key nutrients:**
  - **Sodium** (Maximum 5000 mg/day)
  - **Energy** (Minimum 2000 kcal/day)
  - **Protein** (Minimum 50000 mg/day)
  - **Vitamin D** (Minimum 0.02 mg/day)
  - **Calcium** (Minimum 1300 mg/day)
  - **Iron** (Minimum 18 mg/day)
  - **Potassium** (Minimum 4700 mg/day)
- **Ensure variety** by modifying constraints to prevent reliance on a few food items.

## Methods
The project is implemented using **Python’s PuLP library**.

### **Part 2: Defining the LP Model**
- **Decision Variables**: The number of servings per week for each food item.
- **Objective Function**: Minimize the total weekly cost.
- **Constraints**: Ensure nutrient intake requirements are met.
- **Result**: Very cost-effective but severely lacking in variety.

### **Part 3: Solving the LP Model**
- The model was executed to find the **optimal weekly servings** of each food item at a minimum cost.
- **Result**: The cost was minimized, but the diet consisted of only 3/5 of the food items.

### **Part 4: Adding Variety Constraints**
- Added a new constraint to increase variety: *at least one serving of each food item must be included per week*.
- **Result**: Increased cost very slightly but created a diet with more variety of food items.

### **Part 5: Leveraging a Large Language Model (LLM)**
- **Gemini 2.0** was used to assist in the formation of the linear programming model. 
- **Findings**:
  - The LLM generated useful LP formulations.
  - Definitely needed a bit of guidance, but was capable of completing this simple problem with minimal prompting.

## Results Summary
- The linear programming model successfully created a diet that minimized cost while meeting all nutrient constraints.
- **Variety constraints** improved variety in the diet while increasing the cost minimally.
