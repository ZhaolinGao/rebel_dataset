---
dataset_info:
  features:
  - name: prompt
    dtype: string
  - name: answers
    list:
    - name: answer
      dtype: string
    - name: model
      dtype: string
    - name: rank
      dtype: float64
  - name: turns
    dtype: int64
  - name: num_responses
    dtype: int64
  - name: source
    sequence: string
  - name: good_natured
    dtype: bool
  - name: chat
    list:
    - name: content
      dtype: string
    - name: role
      dtype: string
  - name: oc_chat
    dtype: string
  - name: oc_prompt_tokens
    sequence: int64
  - name: rm_chat
    dtype: string
  - name: rm_tokens
    sequence: int64
  splits:
  - name: train
    num_bytes: 4467625109
    num_examples: 181160
  download_size: 735291303
  dataset_size: 4467625109
configs:
- config_name: default
  data_files:
  - split: train
    path: data/train-*
---
