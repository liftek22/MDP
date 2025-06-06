# MDP
Going through the MDP project from TU_Delft



This link has the original notebook: https://digipedia.tudelft.nl/tutorial/markov-decision-processes/?tab=chapter-0

## 8th May 2025 
Single step decision making 
Sequential decision making

## 9th May 2025
Environment uncertainty  - stochastic environment

State uncertainty - due to partial/noisy environment

## 11th May 2025

MDP are elegant mathmatical framework for the first case (stochastic environments). Can be extended or generalized to cases when we have limited observabilities - this updated framework would be called POMDP.

A Markov chain is a random process/stochastic process) that satisfies the **Markov property**: *Given the current state, the next state is independent of the previous states. *

Mathematically, $\mathbb{P}(s_{t+1} | s_{t}) = \mathbb{P}(s_{t+1} | s_{t}, s_{t-1}, s_{t-2} \ldots)$, where $s_t$ denotes the state of the process at time instant $t$.


## 12th May 2025 

print(f'The outcome of the coin flip is: {flip_coin(face)[0]}')

    This extracts the first (and only) element from the list.

    So if flip_coin(face) returns ['H'], then flip_coin(face)[0] is 'H'.

    Output would be:   
    
  ` The outcome of the coin flip is:  H`

print(f'The outcome of the coin flip is: {flip_coin(face)}')

    This prints the entire list.

    So if flip_coin(face) returns ['H'], then it prints the list as-is.

    Output would be:

   ` The outcome of the coin flip is: ['H']`


   [0] gets us the actual result ('H' or 'T') as a string.

 Without [0], we're printing a list (['H'] or ['T']), which is usually not what wee want for clean output.



## 17th May 2025


    def flip_coin(face):
    
    if face =='H': 
        return random.choices(['H','T'], weights = [0.8,0.2])
    elif face == 'T':
        return random.choices(['T','H'], weights = [0.7,0.3])
    else: 
        print('Incorrect entry!')


For this, the else option does print Incorrect Entry but also gives an error message: 'NonType object is not subscriptable'.  Why? 


GPT Answer: 

because there is no return statement in the else block, the function implicitly returns None.
So you're effectively doing:
print(f'The outcome of the coin flip is: {None[0]}')

'None' is not subscriptable 


Solved the above problem :3 

Return a message - but return it as a list else the result will be just 'I'  - the 0th indexed item of the message. 




## 30th May 2025

Changing color of Markdown text now that `font` is deprecated.  https://stackoverflow.com/questions/19746350/how-to-change-color-in-markdown-cells-ipython-jupyter-notebook

```<span style='color:green'> message/text </span>```

## 6th June 2025 
Spent like an hour trying to different methods to easily launch jupyter notebooks from G drive instead of C.   

Config file changes don't work.  Tried to make a .bat file to use a one click launcher - some DLL error. 

Any, will stick to manually inputting the following in Anaconda Prompth 

    G: 
    jupyter notebook


If I want to go directly to the actual folder, I can do 
    
    G: 
    cd JupyterNotebooks
    jupyter notebook

GPT helped, but was clumsy.  I think I should stick to Gemini. 
