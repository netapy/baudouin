---
Created: 2023-04-03T14:58
---
# Hugging Face 🤗 Course
## Transformer models
### Using Transformers
- On peut importer un modèle sans forcément importer ses weights (à partir du config file, qui indique l’architecture du modèle, le nombre de couches etc…)
### Tokenizers
- 3 différents algorithmes de tokenization
    - **Word based** (1 mot = 1 token)
        - Problèmes : les mots proches sont éloignés, aussi grand que le vocabulaire de la langue (peut être énorme)
    - **Character based** **(1 caractère = 1 token)**
        - Permet un dictionnaire beaucoup plus petit
        - Problèmes : les caractères retiennent peu d’information (dans des langues romanes notamment) **&** réduit le nombre de caractères possibles en input
    - **Sub word based** **(1 mot = plusieurs token, ex : dogs -> dog + s)**
        - permet de regrouper les sous-mots communes d’une langue (comme « ization » ou « iste »)
        - Les mots communs ne sont pas séparés en sous-mots
        - Exemples de models : WordPiece (BERT), Unigram (ALBERT), Byte-Pair Encoding (GPT-2)
### Handling multiple sequences
- Les input doivent toutes avoir la même longueur pour être comparables dans le modèle, il faut donc :
    - Écourter les inputs trop longs (rare, on fixe le maximum comme étant le maximum du modèle)
    - Ajouter des caractères, du « padding » à la fin des petits inputs pour qu’ils arrivent à la taille des grandes.
        - On voit le caractère de padding avec
            
            `tokenizer.pad_token_id`
            
- Les modèles sont souvent limités à 512 ou 1024 tokens et crashent après.
  
### Autres infos de fin
- Le « model head » est le composant qui transforme la prédiction en un output spécifié sur une tâche (traduction, q&a, classification…)
- Le `auto_model` permet de charger la bonne architecture de modèle à partir du checkpoint (weights) uniquement
- On applique le `softmax` à l’output d’un modèle de sequence classification pour
  
  
# Fine-Tuning