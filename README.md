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
1. apply for an access_token of meta-llama/Llama-2-7b-hf (Replace access_token = \<TOKEN\> to your own token.)
2. set the computing process by $ accelerate config default
3. run SFT/sft_llama2.py
4. run DPO/dpo_llama2.py, or RM/reward_modeling_llama.py + PPO/PPO.py
5. run merge_peft_adapter.py


## Acknowledgement
Thanks to the tools and public models on Huggingface!

```
.
├── DPO
│   ├── dpo_llama2.py
│   └── dpo_tuned
├── PPO
│   └── PPO.py
├── RM
│   └── reward_modeling_llama.py
├── SFT
│   ├── results
│   └── sft_llama2.py
├── merge_peft_adapter.py
├── reward_modeling.py
└── README.md
```
