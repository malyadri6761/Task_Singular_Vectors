# Task_Singular_Vectors
One pretrained model and several fine tune models. You want one model doing different tasks retraining on every  data. For resolving retraining process using Task Arithmetic, adding weights from each task, but tasks inference with each other and accuracy drops.



# 1. Paper : Task Singular Vectors Reducing Task Inference arXiv"

**Appendix C.3 has the Theorm 6.1 Proof**

---
## Reducing Task Inference in Model Merging.
---

* **Task Singular Compress(TSV-C)**
```
  Reducing 10% overall size and retaining 90% Accuracy.
```
* **Task Singular Merge(TSV-M)**

  ```
    Merging TSV-Compress Matrices to increasing model merging performance.
  ```
## steps :
1. Considering per-layer matrices& compute SVD.
2. Perform Low-rank approximation.
3. Concatenate the task singular vectors and value.
4. Make the singular vectors orthogonal.
5. Compute the new per-layer task matrix.
