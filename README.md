# RLHF-Llama

## Requirements

evaluate=='0.4.1'

torch=='2.3.0+cu121'

transformers=='4.40.1'

trl=='0.8.6'

typing

peft

accelerate

datasets=='2.17.0'  # '2.19.0' has issues and it does not work!

bitsandbytes

wandb

---

## Steps
1. apply for an access_token of meta-llama/Llama-2-7b-hf (Replace access_token = \<TOKEN\> to your own token.)
2. set the computing process by
```ruby
$ accelerate config default
```
4. run the supervised fine-tuning by "SFT/sft_llama2.py"
5. run DPO by "DPO/dpo_llama2.py", or reward modeling + PPO by "RM/reward_modeling_llama.py + PPO/PPO.py"
6. run "merge_peft_adapter.py" to merge the fine-tuned layers and the original model.


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
└── README.md
```
