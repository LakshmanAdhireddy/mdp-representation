# MDP REPRESENTATION

## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways.

Text representation, Graphical representation, Python - Dictonary representation.

## PROBLEM STATEMENT:

### Problem Description
To conplete the school admisssion process , the role of the agent is to promote if the student is eligible , if not eligible , no admisssion.

### State Space
{A1,A2,A3}->{0,1,2}

A1-> Admission Process 1

A2-> Admission Process 2

A3-> Final Process of Admission

### Sample State
A1 -> Admission Process 1

### Action Space
{E,NE} -> {0,1} E -> Eligible NE -> Not Eligible

### Sample Action
E-> Eligible

### Reward Function
R= { +1, if eligible +0, otherwise

### Graphical Representation
![image](https://github.com/LakshmanAdhireddy/mdp-representation/assets/118707265/8e307103-8cf7-4898-b190-f6b90afeeec5)

## PYTHON REPRESENTATION:
T = {

    0 : {
    
        0 : [(1.0, 1, 1.0, True)],
        
        1 : [(1.0, 0, 0.0, False)]
        
    },
    
    1 : {
    
        0 : [(1.0, 2, 1.0, True)],
        
        1 : [(1.0, 0, 0.0, False)]
        
    },
    
    2 : {
    
        0 : [(1.0, 2, 1.0, True)],
        
        1 : [(1.0, 1, 0.0, False)]
        
    }
    
}

T

## OUTPUT:
![image](https://github.com/LakshmanAdhireddy/mdp-representation/assets/118707265/d614bc50-73d4-44ad-b1c6-2813306523a3)


## RESULT:

Thus the given Markov Decision Process(MDP) problem is represented in the following ways.

Text representation, Graphical representation, Python - Dictonary representation.
