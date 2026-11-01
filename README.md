# Latente : modèles de lecture

Ce dépôt ne contient **aucun code**. Il héberge les fichiers de modèle que l'application Latente télécharge elle-même : Paramètres › Lecteur de bons › Installer.
Vous n'avez rien à télécharger à la main.

## Qwen3.5-2B, moteur « Léger »

Release : [`qwen3.5-2b-b11577`](../../releases/tag/qwen3.5-2b-b11577)

| Fichier | Taille (octets) | SHA-256 |
|---|---|---|
| `Qwen3.5-2B-Q4_K_M.gguf` | 1 312 164 352 | `296b296afb20a6c74229edeb495d99ebf90dcf811756f02f2ed6372b9e0f1e93` |
| `mmproj-Qwen3.5-2B-F16.gguf` | 668 226 688 | `c48336f3768c362981b77559917e8f586a95d50c425cbea2917ad1c0840d47f9` |

L'application vérifie le SHA-256 de chaque fichier après le téléchargement. Un fichier différent est refusé.

## Origine et licence

- Modèle d'origine : [`Qwen/Qwen3.5-2B`](https://huggingface.co/Qwen/Qwen3.5-2B), révision `15852e8c`, par l'équipe Qwen (Alibaba Cloud), sous licence **Apache 2.0** (voir `LICENSE`).
- **Modifications** (voir `NOTICE`) : les fichiers ont été convertis au format GGUF avec `convert_hf_to_gguf.py` de [llama.cpp](https://github.com/ggml-org/llama.cpp), au tag `b11577`.
  - Modèle de langue : quantifié en Q4_K_M avec `llama-quantize`, au même tag.
  - Projecteur d'images (mmproj) : laissé en F16.
  - Aucun réentraînement ni ajustement des poids.
- Ces fichiers sont distribués tels quels, sans garantie, conformément à la licence Apache 2.0.

Publié par Lomirbac Studio Applications (LSA).
