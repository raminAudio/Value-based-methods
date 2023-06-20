
# Banana Navigation

Ramin Anushiravani

### Introduction

This repo contains a value-base method for the banana navigation challenge on Mac. You can train the agent by running "python env.py 1" and you can see the smart agent navigate the banana field by running "python env.py 0". The same code is also included in "Navigation.ipynb", I had problems with running the environment locally, so I run the python script "env.py" instead. 

### You need

[Banana.app](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)\\

Install dependencies,  pip -r requirements.txt

### Codes

Inside "util/" there are three scripts: 
- agent.py : Contains the learning algorithm which implements a dual Deep-QN. 
- qn.py : Contain the Q-Network which implements a double Deep-QN.
- replay.py : Contains the replay buffer. I didn't make any improvements to this code. 


### Artifacts

The final model is saved in the "artifat/checkpoint.pth" along with the plot of all rewards over all episodes "artifact/scores.png" which exceeds 14. 

![plot](artifacts/scores.png)


You can see a short video of the smart agent looking for yellow bananas "artifacts/smart_banana.mov"



### Future Improvements 

Another possible improvement to this balue-based method would be using a "Prioritized experience replay" which should also help smooth the reward, as you can see it's very noisy. Rainbow DQN or a deeper Q-network would also help. Running it for more episodes or generating more data.  







