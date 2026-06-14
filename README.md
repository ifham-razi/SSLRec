# Reproducing SSLRec: A Self-Supervised Learning Framework for Recommendation

This project is for the reproduction of SSLRec [1], a self-supervised learning framework
for recommender systems presented at WSDM 2024. We implement two models from
the framework—LightGCN (the supervised baseline) and SGL (Self-supervised Graph
Learning with contrastive augmentation)—from scratch in PyTorch and evaluate them on the
Gowalla dataset. We describe the full experimental pipeline, diagnose and fix five critical
implementation bugs present in earlier attempts, and compare our reproduced results against
the paper’s reported numbers (Table 3). While our absolute metrics fall below the paper’s
due to dataset-scale and resource constraints, we successfully demonstrate the architectural
validity of SSL-enhanced models and validate the core contrastive learning mechanism. Key
NDCG metrics match or exceed the paper’s values for LightGCN, confirming the correctness
of our evaluation framework.
