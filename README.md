# FIFA Money Ball - AC Milan

This repository contains code for analyzing player data in FIFA 21 and applying the Moneyball concept to identify potential improvements and cost-saving measures for AC Milan.

## Libraries

The code utilizes the following libraries:

* random
* pandas
* numpy
* matplotlib
* re
* seaborn

## Dataset

The code reads a dataset called "fifa21_male2.csv" using pandas and assigns it to the variable `all_players`. This dataset contains information about male players in FIFA 21.

## Problem Definition and Analysis Approach

The code aims to improve the performance of AC Milan while optimizing the budget. The analysis approach focuses on understanding the characteristics of the AC Milan team and identifying areas for improvement.

## Workflow

The code follows the following steps to analyze the dataset:

* Check the available columns in the dataset using `list(all_players.columns)`.
* Obtain an overview of the dataset using `all_players.head()`.
* Perform necessary changes to the dataset, such as converting the 'BP' column to string type and filling missing values with 0.
* Extract the contract start year and end year from the 'Contract' column and store them in separate columns ('start_year' and 'end_year').
* Describe the dataset using `all_players.describe()`.
* Create a filtered dataset called `players_info` by selecting relevant columns from the original dataset. This filtered dataset includes information about player name, age, club, position, potential, value, wage, release clause, total stats, and contract details.
* Plot a correlation matrix using seaborn's `matshow` and `plt.matshow(players_info.corr())`. The matrix visualizes the correlation between different characteristics in the dataset.
* Describe the game strategy used by AC Milan, which is a 4-2-3-1 formation. Explain the roles of different positions on the pitch and how the team transitions between defense and attack.
* Analyze the players in AC Milan based on their positions. Examine the distribution of players in each position, compare the average best overall rating (BOV) of AC Milan players with the general population, and explore the relationship between age and BOV.
* Calculate the wages expense for AC Milan based on the players' wages and store it in `wages_expense`.
* Based on all this information, propose changes to the team to increase the overall best overall rating (BOV) while optimizing the budget.
