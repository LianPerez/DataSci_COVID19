# Daily Probability of Meeting Someone With COVID-19 in Puerto Rico

#### Authors / Programmers:
*   **Facilitator**: Omar Durand Ortiz
*   **Spokesperson**: Ildefonso Pacheco Torres
*   **Quality Control**: Lian M. Pérez Sierra
*   **Process Analyst**: Miguel E. Cruz Molina
#### Instructor: Dr. Patricia Ordóñez Franco
#### Course: CCOM 3031-0U1
#### Date: 12-18-2020

## Introductory description

The Jupyter notebook in this repository contains the code that comprises our calculations and attempt to answer the titular question: what is the probability of meeting someone afflicted with COVID-19 in Puerto Rico? Inspired by Marek Galovič's article ["How likely are you to meet someone with Coronavirus?"](https://towardsdatascience.com/how-likely-are-you-to-meet-someone-with-coronavirus-4522d39487b7), our analysis calculates this probability by using the formula `1 - (1 - P(positive))`, where `P(positive)` is the probability of having the virus. As in Galovič's analysis, our results follow two different statistical approaches towards calculating `P(positive)`, one frequentist and the other Bayesian.

As with other data science projects, our work is comprised by distinct parts devoted to data collection, processing and visualization. Our calculations employ the data recorded by the John Hopkins University of Medicine's [Coronavirus Resource Center](https://coronavirus.jhu.edu/region/us/puerto-rico) for Puerto Rico, which is updated on a daily basis with the exact amounts of new confirmed cases and deaths and total number of tests recorded on the island since the March, 16th. Previous attempts were made to use the data collected by the [Centers of Desease Control and Prevention](https://data.cdc.gov/Case-Surveillance/United-States-COVID-19-Cases-and-Deaths-by-State-o/9mfq-cb36), but said database was eventually considered inadequate, as it didn't include the daily count of negative cases and thus couldn't be used to calculate `P(positive)`. Both dataset extraction processes were included in the final version of the project notebook for replicability purposes.

Finally, after calculating `P(positive)` under both statistical approaches for our dataset, our analysis ends with calculating and displaying the titular probability in two different ways: (1.) plotting the frequentist and Bayesian probabilities of meeting someone with Covid-19 in a group of size *N*, given the probability of having COVID-19 for the last day in the database (i.e. in principle, today), and (2.) plotting the probabilities by time (all the entries in the database from the last to the most recent) for fixed group sizes 3, 6, 9, 12 and 50.

## How to run this project

As with other `.ipynb` files, the notebook comprising this project can be downloaded and run in [Google Colab](https://colab.research.google.com/) or other platforms capable of supporting and opening Jupyter notebooks. It can also be used directly in an already existing Google Colab environment through the following [link](https://colab.research.google.com/drive/1ffJNYpDc_0_tCSlkLjZRaCuzMMLcQgny?usp=sharing). 

## References

* Source article of probability formulas used in this project: ["How likely are you to meet someone with Coronavirus?"](https://towardsdatascience.com/how-likely-are-you-to-meet-someone-with-coronavirus-4522d39487b7), by Marek Galovič

* Datasets:

  * [Coronavirus Resource Center](https://coronavirus.jhu.edu/region/us/puerto-rico) of the John Hopkins University of Medicine
  * [Centers of Desease Control and Prevention](https://data.cdc.gov/Case-Surveillance/United-States-COVID-19-Cases-and-Deaths-by-State-o/9mfq-cb36)

* [Repository of all referenced executive orders](https://www.estado.pr.gov/en/executive-orders/) provided by the Government of Puerto Rico

