# UltimatumGame

* Models the relative outcome of all combinations of offer and reserve price with opponents
* One model generates the offer and reserve prices of the opponents completely randomly and the other uses a normal distribution. 
  + Both models assume the offer and reserve prices are in the range (0, 10) due to human emphasis on fairness and our mutual understanding of this fact.


## Model Proccess:

* First creates all possible combinations of offer and reserve prices. Tests how each of these combinations fairs against opponent values generated either randomly or off of a normal distribution as described above for comparison purposes. 
* Generates 100,000 trials for each possible combination, so in other words re-draws opponent combinations 100,000 times and calculates the total profit of each opponent as well as the total profit for me. 
* Averages my profit and the opponent profit over all of the 100,000 trials. Also generates an average difference value between my profit and my opponents. 
* Therefore we are looking to find the combination of offer and reserve prices that maximizes the difference in my profit and my opponent (highest positive value).

## Output:
* For the opponent combinations generated from a normal distribution, I output a visual of the distribution of offer and reserve prices. 
* As detailed in my report, I select values based on my expectation for opponent behavior/patterns of thought:
  + My selected average opponent reserve = 4
  + My selected average opponent offer =  6 
  + Both use sd = 2 due to my high level of uncertainty in opponent behavior.




