# Loss-in-Food-Supply-Chain

# Identifying which food distribution sector produces the most food waste and modelling the loss percentage

This project hopes to tabulate and model how much Food Loss and Waste (FLW) is produced throughout the Food Supply Chain (FSC). Data collected will be used to train models to predict food loss based on year, country, commodity, and FSC stage. The results will show at which stages of the FSC produces the most and least amount of waste.

This project is developed by: 

Prinz Romeo Gan  (Section: WFY)
Isaiah Nikolo Gonzales (Section: WFY)
Tim Kristian Llanto (Section: WFY)
Gorge Lichael Vann N. Vedasto (Section: WFY)

# Background

Food waste is a significant issue worldwide, with 1.3 billion tons of food lost or wasted every year, according to the Food and Agriculture Organization (FAO) (2018). In the Philippines, the Food and Nutrition Research Institute (FNRI) of the Department of Science and Technology (DOST) states that 1,717 metric tons of food are wasted each day, equivalent to almost twenty-three million Philippine Pesos worth of rice being wasted daily, enough to feed 4.3 million individuals (Pena, K. D., 2021). These losses occur at various stages in the food system, from production to disposal, and can have significant economic, environmental, and social consequences. 

# Materials and Methods

## Materials

Data for this project was obtained from FAO's food loss and waste database [LINK].

## Methods

The following preprocessing steps were applied to the data:

* Data Representation: Extract the necessary columns for this project (commodity, country, year, loss_percent, and food_supply_stage)
* Data Cleaning: remove rows with missing values
* Data Transformation: 
  * Encoding: one-hot encoding will be used for country and commodity features, while label encoding will be used for the column year
  * Scaling: MinMaxScaler method will be used
* Creating Train and Test Data: The dataset for each food supply chain (FSC) stage will be divided into 80:20 ratio for training and testing data
* Model: A linear regression model will be created for each stage in the food supply chain. Each model will take in commodity, country, and year as independent variables and output a loss_percent variable.
* Performance: At least 70% precision for each model
* Visualization: Plot of the linear regression model for each FSC stage

# References

1. Commission for Environmental Cooperation. (2019). Why and how to measure food loss and waste. A practical guide. Montreal, Canada: Commission for Environmental Cooperation. 60 pp.
2. Food Agriculture Organization. (2018) Food Loss and Waste Database. Retrieved 2022 from https://www.fao.org/platform-food-loss-waste/flw-data/en/
3. Patfitt, J., Barthel, M., Macnaughton, S. (2010) Food waste within food supply chains: quantification and potential for change to 2050. doi.org/10.1098/rstb.2010.0126
4. Pena, K. D. (2021) The malady of food waste: millions starve as trash bins fill with leftovers. Inquirer.net . https://newsinfo.inquirer.net/1505252
5. Risenegger, L., Hubner, A. (2022) Reducing food waste at retail stores an explorative study. 14, 2294, doi.org/10.3390/su14052595
