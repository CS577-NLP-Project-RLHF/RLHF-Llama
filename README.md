# RLHF-Llama

## Requirements

evaluate

torch

transformers

trl

typing

peft

accelerate

datasets==2.17.0

bitsandbytes

wandb

warnings

---

## Steps
1. apply for an access_token of meta-llama/Llama-2-7b-hf
2. set the computing process by $ accelerate config default
3. run SFT/sft_llama2.py
4. run DPO/dpo_llama2.py, or RM/reward_modeling_llama.py + PPO/PPO.py
5. run merge_peft_adapter.py
