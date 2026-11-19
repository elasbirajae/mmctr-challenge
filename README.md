MM-CTR Challenge - Task 1 et 2 
# MM-CTR Challenge - Task 1 + 2

Projet de Web Analytics : participation au Multimodal CTR Prediction
Challenge (WWW 2025 EReL@MIR Workshop), sur le dataset MicroLens-1M.

## Approche (Task 1 + Task 2 en cascade)
- **Task 1 - embeddings d'items** : embeddings d'images CLIP (ViT-B/32, 512 dim)
  concaténés avec un vecteur de tags (SVD, 32 dim), puis PCA en 128 dimensions
  (83 % de variance conservée).
- **Task 2 - modèle CTR** : DIN (baseline FuxiCTR), entraîné avec les embeddings
  d'origine puis avec les nôtres.

## Notebooks Kaggle
- Task 1 : mmctr-task1-embeddings
- Task 2 : mmctr-task2-ctr

## Résultats (AUC de validation)
| Expérience | AUC |
|---|---|
| Baseline (embeddings d'origine) | à compléter |
| Nos embeddings (Task 1) | à compléter |

## Références
- Baseline : https://github.com/reczoo/WWW2025_MMCTR_Challenge
- Challenge : https://erel-mir.github.io/challenge/mmctr-track2/