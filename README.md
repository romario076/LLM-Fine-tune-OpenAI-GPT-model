### Fine tuning LLM GPT-3.5-turbo with own data using OpenAI

In this notebook described how to fine tune openai model with own data.
For this neccessary to have openai api key, to be abble to work with gpt model.

In .env file put your openai api key.

<img width="574" alt="image" src="https://github.com/user-attachments/assets/e42c9cc0-a598-471c-a03e-fcabedcc4647">


Data set contains 2235 rows and 2 columns. For fie tunning not neccessary to have very large data set, firstrly it will cost a lot and secondly better to have small data set but more reliable.
Data set designed for classification problem. It has text and corresponding category of this text: sport, politics, entertainment, business, tech. This category we will try to predict using gpt model.

Data set:

<img width="787" alt="image" src="https://github.com/user-attachments/assets/f2551e4e-57f0-4360-b341-ed94c561f1f6">

We will use "text" column from the data set as input abd "category" as target variable for classification.
In the notebook we will compare base GPT-3.5-turbo model with fine tuned GPT-3.5-turbo on this data set and will compare theirs perfomance.

For demonstration was selected very small data set for fine tunning to save costs. 
You can use openai pricing to calculate how much it will cost to train and evaluate model depends on data set size. In notebook formula is provided. 
If you want to see fine tunning influence more significant on the result, please increse train and test data set size in notebook, but be aware that costs will increase.
