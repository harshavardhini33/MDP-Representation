# MDP REPRESENTATION

## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways.

1) Text representation
2) Graphical representation
3) Python - Dictonary representation
## PROBLEM STATEMENT:
* To develop an environment in which a person is hiking in a mountain. The goal is to reach the top of the mountain
  
## PROBLEM DESCRIPTION:
* The agent has to reach the goal state(top of mountain) by taking the correct step towards the goal without drifting away from the path. After reaching the goal the agent will be rewarded if not then no reward will be provided.

## State Space:
{0,1,2,3,4}

## Sample State:
0 -> Starting point(S)
1 -> Relaxing point(R)
2 -> View point(G)
3 -> Dangerous point(D)

## Action Space:
 {1,2}

## Sample Action:
1 -> Moving up
2 -> Moving down
## Reward Function:
```
if Agent reached Goal(G) state:
       reward=+1
else
       reward=0
```
### Graphical Representation
![image](https://github.com/gpavithra673/mdp-representation/assets/93427264/0b923bf1-eeef-4ea1-b4b0-2aff0392bf67)


## PYTHON REPRESENTATION:
```
Hiking = { 
    #starting point state(S) ->0
    #Action: up-> 1, down-> 2
  0:{
     1:[(0.82 , 1 , 0,False),(0.18 , 0 , 0 , False)],
     2:[(0.88 , 0 , 0,False),(0.12 , 1 , 0 , False)] 
  },
    #relaxing point state(R) ->1
  1:{
     1:[(0.91 , 2 , 0,False),(0.09 , 0 , 0 , False)],
     2:[(0.75 , 0 , 0,False),(0.25 , 2 , 0 , False)]
  },
    #View point state(G) ->2
  2:{
      1:[(0.92 , 3 , 1,True),(0.08 , 1 , 0 , False)],
      2:[(0.91 , 1 , 0,False),(0.09 , 3 , 1 , True)]
  },
    #Dangerous point state(DD) ->3
  3:{
      1:[(0.82, 3 , 0, True),(0.18 , 2 , 0 , False)],
      2:[(0.73, 2 , 0, False),(0.27 , 3 , 0 , True)]
  }
}
Hiking
```
## OUTPUT:
![image](https://github.com/gpavithra673/mdp-representation/assets/93427264/017ee6de-ec59-4296-b832-979e80f13e89)

## RESULT:
### Hence we have created an environment suitable for the above mentioned problen.

