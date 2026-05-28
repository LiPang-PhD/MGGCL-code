# MGGCL: Motif-Guided Graph Contrastive Learning for Recommendation

This repository contains the source code for the paper **"MGGCL: Motif-Guided Graph Contrastive Learning for Recommendation"**.

---

## 📁 Code Archive Information

Due to file size constraints, the full code has been split into **9 separate zip files**:
- `MGGCL_part01.zip`
- `MGGCL_part02.zip`
- `MGGCL_part03.zip`
- `MGGCL_part04.zip`
- `MGGCL_part05.zip`
- `MGGCL_part06.zip`
- `MGGCL_part07.zip`
- `MGGCL_part08.zip`
- `MGGCL_part09.zip`

### How to Reconstruct the Full Code
1. Download all 9 zip files to the same directory
2. On macOS/Linux, run the following command in terminal:
   ```bash
   cat MGGCL_part*.zip > MGGCL_full.zip && unzip MGGCL_full.zip

### Code Structure Overview
main.py
├── argparse
├── ModelConf()
├── SELFRec(conf)
│   ├── load train/test
│   └── preprocess
└── rec.execute()
    └── SELFRec.execute()
        ├── dynamic import model
        ├── create model object
        └── model.execute()
            ├── train()
            │   ├── sample batch
            │   ├── GNN propagation
            │   ├── motif propagation
            │   ├── contrastive loss
            │   ├── BPR loss
            │   └── optimizer.step()
            └── evaluate()
