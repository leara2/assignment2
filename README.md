# Complex Systems group assignment 2: Replicate and plot a model of a chosen paper


### Overview
This project replicates parts of the mathematical proofs by Clark (1973), showing how the sole owner of a resource might decide that it is optimal to harvest named resource to extinction if they consider the immediate revenue from harvesting to be sufficiently high compared to future harvesting revenue. The math introduced in the paper and the criteria Clark gives for the functions are used. Figure 3a (intermediate price) and 3b (high price) are recreated as well as a simulation of the effect of the discount rate (α) on f'(x) to show how the introduction of alpha can make an optimum intersection point between sustainable species growth and profit maximisation disappear, making it the most rational choice for the owner of the resource to harvest remaining animals to extinction. 

### The Model
The model combines a growth function with an economical harvesting function.

Population growth is modelled by: 
  f(x)= x + r*x*(1 - x/K)
**x** is the current population, **r** the growth parameter and **K** the carrying capacity of the environment

Marginal net revenue from harvesting is depicted as
  M'(x) = p - g(x)
**p** is the price of the resource and **g(x)** is representing the harvesting cost per unit
  g(x) = c/(x+1), where **c** is the cost of harvesting one unit from population x+1 

Actual profit of harvesting a unit when population is x / actual profit of harvesting a unit when population x has reproduced and gave a new amount of population

The economic value of an animal today compared with the value of the population it helps produce next period is therefore depicted as
M'(x)/ Μ'[f(x)]

### Visualisation
The code visualises Figure 3a and b depicting profit maximisation at different price rates. It also allows to see how alpha varies and at which point of the function the maximum revenue can be achieved by harvesting the entire resource.

### Requrements
*Installations*
pip install numpy matplotlib scipy pillow

### How to Run

1. Download or clone the repository.
2. Install the dependencies.
3. Run the Python script or notebook.


### References
Clark, C. W. (1973). Profit Maximization and the Extinction of Animal Species. Journal of Political Economy, 81(4), 950–961. http://www.jstor.org/stable/1831136
