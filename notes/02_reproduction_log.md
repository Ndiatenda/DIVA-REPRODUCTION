# DIVA Reproduction Log

## Smoke test: supervised rotated MNIST

Branch: smoke-test-local  
Base branch: baseline-diva  

Command:

```bash
cd paper_experiments/rotated_mnist/supervised
PYTHONPATH=../../.. python experiment_only_sup_diva.py --epochs 5