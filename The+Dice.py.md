
# The Dice Program

First we import the Random Package that allows us to get random responses:


```python
import random
```

Then we create the function that is going to be our dice:


```python
# adding the variables that will need to be added to the function later on.
def dice(min,max): 
    print("Rolling the dices...")
    
    # printing out a random number between min and max. 
    print("You Rolled: " + str(random.randint(min, max))) 
```

Then We need a variable for if we want to run the code again Yes or No:


```python
roll_again = "yes"
```

Then we add in the while loop that is going to repeat the dice as long as we respond with 'yes' or 'y'
it will ask the user for an interval divided by (``-``) so a ``1-6`` means between ``1`` and ``6``.


```python
# while loop that is going to repeat the dice as long as we respond with 'yes' or 'y'
while roll_again == "yes" or roll_again == "y": 
    
    # ask the user for an interval divided by (-)
    interval_input = input("Interval: ")  
     
        # splits the input by the divider (-)
    interval = interval_input.split('-')
    
    # sets the value before (-) in the interval[0] 
    # and the value after (-) in the interval[1]
    dice(int(interval[0]),int(interval[1])) 
    
    #ask the user for a 'yes', 'y' or no to repeat the dice
    roll_again = input("Roll the dices again? ")
```

    Interval: 1-6
    Rolling the dices...
    You Rolled: 6
    Roll the dices again? yes
    Interval: 1-100
    Rolling the dices...
    You Rolled: 26
    Roll the dices again? no
    


```python

```
