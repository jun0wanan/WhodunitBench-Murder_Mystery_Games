# WhodunitBench-Murder_Mystery_Games
[NeurIPS2024-D&amp;B-spotlight]: WhodunitBench: Evaluating Large Multimodal Agents via Murder Mystery Games
![preview](./demo.gif)


## News
🔥 Dataset content has been updated, with full updates to be completed during the May Day holiday period.

## Table of Contents

- [Requirements](#requirements)
- [Evaluation](#evaluation)
- [Data Structure](#data-structure)

## Requirements
Run the following command to install the required packages:
```bash
 conda env create -f environment.yaml
```

## Evaluation
```bash
python GameStart.py --name GPT4V  --type naive_agent  --root_file  your_data_file(eg.Data)   --save_file  save_model_file
```

## Data Structure
The data structure for one script is as follow:
```
+--img: all the image clues
+--env_p_all.json
| +--key_clues_pool: Contents of reasoning at different stages.(eg. 1-step)
| +--public_clue : all the text clues
| +--key_clues_questions ：all the cognition qa
| +--a: the first role, including its name and LS-qa, etc.
| +--role: all the roles of this script
| +--ei_q: all the text-rich image qa
| +--cxi_q: all the media-rich image qa
| +--reason: the motive and method of this script
| +--murder: the murderer of this script
| +--key_role: all the key_role of this script
```
