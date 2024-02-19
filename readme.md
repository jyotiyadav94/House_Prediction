# Project Overview

## Description
The project aims to analyze and predict house prices using machine learning techniques. The dataset includes various features related to residential properties, such as area, amenities, and location. By leveraging this dataset and employing machine learning algorithms, the goal is to build a predictive model that can accurately estimate the sale price of houses.

# Dataset Description

## File Descriptions
- `train.csv`: The training set
- `test.csv`: The test set
- `data_description.txt`: Full description of each column, originally prepared by Dean De Cock but lightly edited to match the column names used here
- `sample_submission.csv`: A benchmark submission from a linear regression on year and month of sale, lot square footage, and number of bedrooms

## Data Fields
Here's a brief version of what you'll find in the data description file:

- `SalePrice`: The property's sale price in dollars. This is the target variable that you're trying to predict.
- `MSSubClass`: The building class
- `MSZoning`: The general zoning classification
- `LotFrontage`: Linear feet of street connected to property
- `LotArea`: Lot size in square feet
- `Street`: Type of road access
- `Alley`: Type of alley access
- `LotShape`: General shape of property
- `LandContour`: Flatness of the property
- `Utilities`: Type of utilities available
- `LotConfig`: Lot configuration
- `LandSlope`: Slope of property
- `Neighborhood`: Physical locations within Ames city limits
- `Condition1`: Proximity to main road or railroad
- `Condition2`: Proximity to main road or railroad (if a second is present)
- `BldgType`: Type of dwelling
- `HouseStyle`: Style of dwelling
- `OverallQual`: Overall material and finish quality
- `OverallCond`: Overall condition rating
- `YearBuilt`: Original construction date
- `YearRemodAdd`: Remodel date
- `RoofStyle`: Type of roof
- `RoofMatl`: Roof material
- `Exterior1st`: Exterior covering on house
- `Exterior2nd`: Exterior covering on house (if more than one material)
- `MasVnrType`: Masonry veneer type
- `MasVnrArea`: Masonry veneer area in square feet
- `ExterQual`: Exterior material quality
- `ExterCond`: Present condition of the material on the exterior
- `Foundation`: Type of foundation
- `BsmtQual`: Height of the basement
- `BsmtCond`: General condition of the basement
- `BsmtExposure`: Walkout or garden level basement walls
- `BsmtFinType1`: Quality of basement finished area
- `BsmtFinSF1`: Type 1 finished square feet
- `BsmtFinType2`: Quality of second finished area (if present)
- `BsmtFinSF2`: Type 2 finished square feet
- `BsmtUnfSF`: Unfinished square feet of basement area
- `TotalBsmtSF`: Total square feet of basement area
- `Heating`: Type of heating
- `HeatingQC`: Heating quality and condition
- `CentralAir`: Central air conditioning
- `Electrical`: Electrical system
- `1stFlrSF`: First Floor square feet
- `2ndFlrSF`: Second floor square feet
- `LowQualFinSF`: Low quality finished square feet (all floors)
- `GrLivArea`: Above grade (ground) living area square feet
- `BsmtFullBath`: Basement full bathrooms
- `BsmtHalfBath`: Basement half bathrooms
- `FullBath`: Full bathrooms above grade
- `HalfBath`: Half baths above grade
- `Bedroom`: Number of bedrooms above basement level
- `Kitchen`: Number of kitchens
- `KitchenQual`: Kitchen quality
- `TotRmsAbvGrd`: Total rooms above grade (does not include bathrooms)
- `Functional`: Home functionality rating
- `Fireplaces`: Number of fireplaces
- `FireplaceQu`: Fireplace quality
- `GarageType`: Garage location
- `GarageYrBlt`: Year garage was built
- `GarageFinish`: Interior finish of the garage
- `GarageCars`: Size of garage in car capacity
- `GarageArea`: Size of garage in square feet
- `GarageQual`: Garage quality
- `GarageCond`: Garage condition
- `PavedDrive`: Paved driveway
- `WoodDeckSF`: Wood deck area in square feet
- `OpenPorchSF`: Open porch area in square feet
- `EnclosedPorch`: Enclosed porch area in square feet
- `3SsnPorch`: Three season porch area in square feet
- `ScreenPorch`: Screen porch area in square feet
- `PoolArea`: Pool area in square feet
- `PoolQC`: Pool quality
- `Fence`: Fence quality
- `MiscFeature`: Miscellaneous feature not covered in other categories
- `MiscVal`: $Value of miscellaneous feature
- `MoSold`: Month Sold
- `YrSold`: Year Sold
- `SaleType`: Type of sale
- `SaleCondition`: Condition of sale

## Classes

### Class I: HouseObjectOriented Class
- Adds the data to the object
- Concatenates the data into one DataFrame
- Shows information about the data
- Preprocesses the data before the ML part
- Adds the data after preprocessing for the ML part

### Class II: Information Class
- Calculates the missing values
- Gets feature dtypes
- Gets feature names
- Gets shape of the data
- Prints all of these information

### Class III: Pre-processing Class
- Drops the unwanted columns and rows
- Fills the null values with (mean, median, zero, etc.)
- Applies feature engineering to the data like adding new columns, transforming columns, etc.
- Encodes the data using label encoder to be able to apply ML algorithms
- Converts your data to dummy values
- Normalizes the data before ML

### Class IV: Preprocessor Class
- Applies the preprocessing techniques and returns the new data

### Class V: ML Class
- Initializes the ML algorithms
- Shows the available ML algorithms
- Applies Train-Test evaluation and shows the results
- Applies Cross-Validation evaluation and shows the results
- Visualizes the results of Train-Test and Cross-Validation evaluations
- Finds the best model and then fits it to the data
- Shows the predictions in a DataFrame
- Saves the predictions to a CSV file
