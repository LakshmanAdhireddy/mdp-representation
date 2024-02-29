 MDP REPRESENTATION

## AIM:
To represent any one real-world problem in MDP form.

## PROBLEM STATEMENT:

### Problem Description
Consider an AI agent optimizing elevator operation in a high-rise building to efficiently transport passengers between floors.

### State Space
state_space = {
"Elevator1": 0,  

"Elevator2": 1,

"Elevator3": 2,  

"PassengerWaiting": 3  
}
### Sample State
sample_state = "Elevator1 -> 5"

### Action Space
action_space = { "MoveUp": 0,

"MoveDown": 1,

"OpenDoors": 2,

"CloseDoors": 3  
}

### Sample Action
sample_action = "MoveUp -> 0"

### Reward Function
reward_function = { "PassengerServed": +1,

"EfficientOperation": +0.5,  

"EmptyTrips": -0.5  
}

### Graphical Representation
![image](https://github.com/LakshmanAdhireddy/mdp-representation/assets/118707265/1ffefc2a-debe-4ad8-987c-1fb17de06f7a)

## PYTHON REPRESENTATION:
P = {

    0: {
    
        0: [(0.9, 0, 1, False), (0.1, 1, 0, False)],
        
        1: [(0.1, 0, 1, False), (0.9, 1, 0, False)],
        
        2: [(0.0, 0, 0, True)],
        
        3: [(0.0, 0, 0, True)]
        
    },
    
    1: {
    
        0: [(0.1, 0, 1, False), (0.9, 2, 0, False)],
        
        1: [(0.9, 0, 1, False), (0.1, 2, 0, False)],
        
        2: [(0.0, 1, 0, True)],
        
        3: [(0.0, 1, 0, True)]
        
    },
    
    2: {
    
        0: [(0.1, 1, 1, False), (0.9, 2, 0, False)],
        
        1: [(0.9, 1, 1, False), (0.1, 2, 0, False)],
        
        2: [(0.0, 2, 0, True)],
        
        3: [(0.0, 2, 0, True)]
        
    },
    
    3: {
    
        0: [(1.0, 3, 0, True)],
        
        1: [(1.0, 3, 0, True)],
        
        2: [(1.0, 3, 0, True)],
        
        3: [(1.0, 3, 0, True)]
        
    }
    
}

## OUTPUT:
![image](https://github.com/LakshmanAdhireddy/mdp-representation/assets/118707265/98f20d3b-8067-4e8f-9731-e95de6e2468c)

## RESULT:
Thus the given real world problem is successfully represented in a MDP form .
