# MDP REPRESENTATION

## AIM:
To represent any one real-world problem in MDP form.

## PROBLEM STATEMENT:

### Problem Description
Imagine a small room with a heater and a cooler. Your goal is to develop a control system to keep the room's temperature as close to a desired temperature as possible while minimizing energy consumption.

### State Space
The state is determined by the room's current temperature.

### Sample State
For example, the room's current temperature is 70°F.

### Action Space
There are two actions:
1. Turn on the heater 
2. Turn on the cooler

### Sample Action
You decide to turn on the heater.

### Reward Function
* Positive reward for the temperature being close to the desired temperature.
* Negative reward for high energy consumption.
* Negative reward for the temperature being far from the desired temperature.

### Graphical Representation
Write your answer here

## PYTHON REPRESENTATION:
```
Developed by Harshavardhini on 29th of Aug '23
```
```
P={0: {0: [(1.0, 0, 0.0, True)],
       1: [(1.0, 0, 0.0, True)]},
   1: {0: [(1.0, 0, 0.0, True)],
       1: [(1.0, 2, 1.0, True)]},
   2: {0: [(1.0, 2, 0.0, True)],
       1: [(1.0, 2, 0.0, True)]}}
```

## OUTPUT:
Write your Python output here

## RESULT:
Write your output here

