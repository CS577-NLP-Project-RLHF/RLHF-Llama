
## Steps
1. apply for an access_token of meta-llama/Llama-2-7b-chat-hf
2. 
```
pip install -r requirements.txt
```
4. train the reward model 
```
python reward_modeling.py
```
5. run PPO with 
```
python ppo_trainer.py
```