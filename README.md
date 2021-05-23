
# Advanced-Algorithms
- **By** Benamara Abdelkader Chihab   &   Djelid Aymen

**Advanced-Algos** is  our course assignement for the first semester at Paris Dauphine University. It is composed of 2 main algorithms in which all this 4 types of algorithms were achieved : `Greedy Algorithms `,`Dynamic Programming` , `Divide & Conquer`and `Branch & Bound`.
This 2 subjects were about **Discrete Unit Disc Cover Problem (DUDC)** and **Upper Envelope Problem (UEP)** and we were able to make `pseudo-code` for all of this methods but for now we implemented **`DUDC Problem`** in **1D** and **2D**. Coming soon **UEP**

## Discrete Unit Disc Cover Problem (DUDC)
### Implementation in 1-dimension 
For this version of **`DUDC`** we were able to solve it with a greedy algorithm and we proved the optimality of this greedy choice.
**Greedy Choice :** Sort all points from left to right  and do the same for the unit circles ,  and when looping throw the points we will take the right-most circle that contains this actual point and after that we need to remove all other points which are covered by the taken circle.
### Implementation in 2-dimensions
For this version of **`DUDC`** we were able to solve it with a branch & bound algorithm in which we used two bounds :
1. Upper Bound ( **`UB `** ) : The size of actual solution ( if we've taken 3 circles until now then **`UB`**= 3
2. Lower Bound ( **`LB `** ) : Here we created an algorithm to estimate the best solution which we can afford from the actual **`NODE`** in the tree This bound was calculated by this algorithm : 
![LB](https://user-images.githubusercontent.com/38104305/105034650-10c78600-5a5a-11eb-88e3-0032733258e5.JPG)
3. For The branching method we used the basic one which stand on two possible choices for any node ( we can take it or not ) 
4. The Sterilisation is also handled the basic way : 
4.1. If the actual solution is not possible ( a point can't be covered by no one of the **Q*** 
4.2. If we already have a solution with a lower bound or equal 

**PS :** The pseudo-code is available   [here](https://github.com/ChihabEddine98/AdvancedAlgos/blob/main/APA_rapport.pdf)
and  the implementation [here](https://github.com/ChihabEddine98/AdvancedAlgos/blob/main/DUDC/DUDC.ipynb)

TODO -- 
1. Code UEP
2. Optim DUDC 2D B&B
