# Markov Process
# Aim : 

![image](https://user-images.githubusercontent.com/75235150/171331821-5a16c33c-1938-4b23-ac66-c122aeccaa11.png)

# Software required :  

Python

# Theory:

Markov chains, named after Andrey Markov, a stochastic model that depicts a sequence of possible events where predictions or probabilities for the next state are based solely on its previous event state, not the states before. In simple words, the probability that n+1th steps will be x depends only on the nth steps not the complete sequence of steps that came before n. This property is known as Markov Property or Memorylessness. 

Assumptions for Markov Chain :
1. The statistical system contains a finite number of states.
2. The states are mutually exclusive and collectively exhaustive.
3. The transition probability from one state to another state is constant over time.
# Procedure :

![image](https://user-images.githubusercontent.com/75235150/171331839-f3ad19af-a1cb-4a76-9881-499df5147d69.png)

# Program

```python
import numpy as np
p0 = [0.3,0.2,0.5]
p = [[0,2/3,1/3],[1/2,0,1/2],[1/2,1/2,0]]
n=6
for i in range(1,n+1):
    p0 = np.multiply(p0,p)
    print("The %d -step probability distribution is &"%i)
    print(p0)
```
# Output : 

![image](https://user-images.githubusercontent.com/75235150/171331862-14eeebea-309b-4bc3-a0d1-0765d6c84147.png)

# Results :
Thus the n-step probability distribution matrix using Markov's Process has been found.
