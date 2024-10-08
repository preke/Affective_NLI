# Affective-NLI

## Data Construction


### FriendsPersona

1. `data/Friends_Persona.py`: construct unlabeled tsv data in each single dimension
2. `data/label_friends_persona_with_emoberta.py`: labeling utterance with basic emotion labels
3. `data/Friends_Persona_NLI_construction.py`: construct NLI data with different dialog flow lengths


### CPED

- `data/CPED_construction.ipynb`: construct NLI data with different dialog flow lengths

## Affective-NLI

You have to construct dataset first then run the following code

- `src/affective_nli_roberta.py`: Run with RoBERTa
- `src/affective_nli_T5.py`: Run with T5
- `src/affective_nli_llama.py`: Run with llama2-7b 




The above three scripts share similar structures; dataset, random seeds, dialog length, and hyperparameters can be modified in the main function (`if __name__ == '__main__':`).

## Requirements

- `pytorch==1.13.0` or higher
- `transformers==4.23.1` or higher
- `openprompt==1.0.1`
