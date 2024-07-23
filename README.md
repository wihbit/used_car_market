# Used Car Market
# Project 1 - Exploratory Data Analysis and Visualization

## Project Overview  
In this project, we set out to find a dataset, perform initial data cleaning operations, and then impliment exploratory and statistical data analysis techniques to answer important questions about the data, with real world implications.

In our case, we chose a dataset containing information on used car auctions, which gives insight into the value of used cars from a wide range of years, makes, models, and conditions.

After previewing the data, we decided that we want to be able to answer the following questions:
1. How do used cars depreciate?  
    - By mileage, overall?
    - By body type?
    - By make?
2. What are the highest and lowest selling cars?
3. Do certain states and regions have unique patterns for used cars?

## Usage/Installation

Recommended python version: `>= 3.11.7`  
Required packages/libraries:  
- pandas: `pip install pandas`  
- matplotlib: `pip install matplotlib`  
- seaborn: `pip install seaborn`  
- scipy: `pip install scipy`  
- plotly: `pip install plotly`  
- numpy: `pip install numpy`  
- datetime: `pip install datetime`  

## Files
- alex.ipynb
    - Jupyter notebook for EDA and visualizations
    - Related to the question: How do used cars depreciate?
- esteban.ipynb
    - Jupyter notebook for EDA and visualizations
    - Related to the question: Do certain states and regions have unique patterns for used cars?
- Project_1_Chuckspart.ipynb
    - Jupyter notebook for EDA and visualizations
    - Related to the question: What are the highest and lowest selling cars?
- data_cleaning.ipynb
    - Jupyter notebook for data ingest and cleaning
- final_clean_car_data.csv
    - CSV of the data post-cleaning
- README.md
    - The project's README document

## Analysis Summary  

### How do used cars depreciate?  
**By mileage:**  
- Used cars steadly lose value as mileage and age increase
- Averaging data across all years, makes, and models, cars lose about $1,200 in value per 10,000 miles  

**By body type**
- For all car body types, the steepest rate of depreciation is during the first 100,000 miles
- After 100,000 miles, the rate of depreciation gradually diminishes
    - *Speculation: After 100,000 miles, there isn't much farther for the value to sink, and there is probably less difference in risk/reward between owning a high mileage car vs a VERY high mileage car.*
- Trucks have the lowest rate of depreciation overall
- Although counterintuitive, it appears that trucks and vans have a tendency to *appreciate* in their first 25,000 miles, before depreciating like normal.  
- Although not by a huge margin, convertibles, coupes, and vans depreciate the fastest
    - *Speculation: What convertibles, coupes, and vans all have in common is that they are niche vehicles. Coupes and convertibles are more sporty and stylish than practical, and vans are practical, but for less common purposes. That may be why they depreciate faster: less of an audience for them.*

**By make**
- Mazdas in the dataset had the fastest depreciation rate
- GMCs in the dataset had the slowest depreciation rate
    - *Speculation: GMC mostly makes trucks, and trucks in general depreciate slower than the others, which probably explains why they came out on top. Trucks are skewing the data*
- The 4 next slowest depreciating makes (Toyota, Ford, Chevrolet, Nissan) all happen to be the top 4 selling cars in the dataset
    - *Speculation: What comes with selling so many cars is having a robust parts & maintenance network around the country. People who buy these brands know it is not hard to find parts (OEM or aftermarket) and service centers (official dealerships or third party specialists). That may explain why they depreciate relatively slowly: they are better maintained because they make it easy to do so.*

### What are the highest and lowest selling cars?  

### Do certain states and regions have unique patterns for used cars?
