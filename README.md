# UltimatumGame

* Models the relative outcome of all combinations of offer and reserve price with $20 pot and 18 players including self.
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

![Offer](https://user-images.githubusercontent.com/65736586/132957825-6c2020dd-7978-4921-9404-8578aca108b9.png)
![Reserve](https://user-images.githubusercontent.com/65736586/132957826-7c65cac1-3ee5-457a-9242-63841c9c6fc1.png)

* For each combination I output a plot showing my total profit, opponent average profit, and difference in profit over 100,000 trials: 
 ![Comparison](https://user-images.githubusercontent.com/65736586/132957851-d0664520-8593-4fed-9dd6-8c18b2c3857b.png)


* For each combination I output the distribution of the difference in profits. The average of that value is what I use to ultimately select the best model.
 ![Histogram](https://user-images.githubusercontent.com/65736586/132957874-fc78488c-1987-4639-81f3-bf2d916f4132.png)

* The difference data for each possible combination is outputted numerically and can be found in the repository files. 

## Results:
* I compare the results of the randomly generated samples as well as the samples generated from a normal distribution to ultimately determine which combination is most likely to outperform those of my opponents. I visualize the 3 dimensional data as a heatmap: 

#### Randomly Generated: 
![randomheatmap](https://user-images.githubusercontent.com/65736586/132958485-476c19d6-d2c9-494e-be88-09050dd40cb2.png)


#### Normal Distribution Generated:
![normalheatmap](https://user-images.githubusercontent.com/65736586/132958488-36360853-b105-42af-a7c2-448ff2005a45.png)






