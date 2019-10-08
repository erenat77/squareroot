# The squareroot function in python

* The square root function by using a well-known technique called “Newton’s Method.”
* Newton’s Method for approximating square roots performs an iterative computation that converges on the correct value. 
**The equation** is `$$newguess=(1/2)∗(oldguess+(n/oldguess)$$` 

* It takes a value n and repeatedly guesses the square root by making each newguess the oldguess in the subsequent iteration. The initial guess used here is `n/2`

* Here is the python code:
```python
def squareroot(n):
    root = n/2    #initial guess will be 1/2 of n
    for k in range(20):
        root = (1/2)*(root + (n / root))

    return root
```
    
