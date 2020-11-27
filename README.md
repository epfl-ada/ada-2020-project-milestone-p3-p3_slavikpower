# You are what you eat - Relating Demographic Data to Food Consumption Habits

# Abstract

The original paper presents the Tesco Grocery 1.0 data set and verifies the data by correlating the typical food product with the prevalence of different metabolic diseases.
We are interested in the influence of demographic data on food composition, more specifically, we want to predict the contents of the typical food product of each ward by demographic markers such as gender, age, race, and wealth.
The UK government provides ward profiles with the aforementioned demographic markers. We can merge the grocery data and the demographic data by the ward identifiers. To explore the interplay between demographic data and food consumption habits, we first explore the data and conduct a correlation analysis.
Afterward, we build a model that, given demographic markers, predicts the contents of the typical food product consumed in a ward.
Lastly, we plan to explore the validity of our model. Our analysis would allow us to better understand the consumption habits of different population groups.

# Research questions

1. What is the relation between each individual demographic marker and food consumption habits?
2. How well can we predict food consumption habits from demographic markers?
3. How does data representativeness affect our model performance?

# Proposed datasets

[Tesco Grocery 1.0 from the paper](https://figshare.com/collections/Tesco_Grocery_1_0/4769354/2) -- this dataset provides the nutrients of the typical food product on different spatial granularities.
[Ward Atlas](https://data.london.gov.uk/dataset/ward-profiles-and-atlas) -- this dataset provides several demographic features at the ward level.
Specifically, we will use gender, wealth, age, and race.

# Methods

*Data collection*: enrich the Tesco dataset with demographic data from the Ward Atlas dataset.

*Data analysis*: Once we have demographic data and food datasets merged we will proceed to the analysis of correlations among different properties groups we are interested in, i.e. dependence of protein consumption on median income.
After exploring the correlations we will build our model, which should predict the distribution of meal constituents on demographic data for every area. 

*Building the model*: we will build a neural network to predict the typical food product’s ingredients
 We are going to explore different model configurations, i.e. Loss functions and activation functions.

*Validation*: We study the dependence of the model’s loss on the representativeness of the training data. 

# Proposed timeline
- Week 1: Downloading and merging the data sets, doing a sanity check. Search for the correlations and visualize properties
- Week 2: Build the model that should predict consumption habits from demographic markers.
- Week 3: Study performance of the models obtained, prepare data story 

# Organization within the team
- Alex does the data merging and data exploration
- Denys and Egor build the model and study the representativeness
- Everyone writes about their part in the data story

