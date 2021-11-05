# [Deep medical image registraiton: a survey](https://link.springer.com/content/pdf/10.1007/s00138-020-01060-x.pdf)

!!! : 3 problem for DL in registration:
    1. **multimodal image:**
       + different fields of view -> hard to extract control point
    2. **deformable registration:**
       + dim of parameters -> high: hard to train/ low: too weak to register S to T
       + constrain of deformation fields -> realistic organ appearence
    3. **grand truth:**
        + real data -> hard to get
        + simulated data -> differet from real

![](picture/2021-11-05-16-10-38.png)

## 1. Deep iterative registration

### 1.1 Deep similarity-based registration

![](picture/2021-11-05-16-25-02.png)

Method use CNN to learn a deep similarity metric, than the metric is inserted into classical registration frameworks.

### 1.1.1 unimodal registration

Deep similarity based methods can't outperform mannually crafted methods. However, it can complement information.

### 1.1.2 multimodel

