---
title: "Covariance propagation for attitude-only ESKF"
tags: [estimation, robotics, math]
math: true
---

We propagate quaternion covariance as:

$$
P_{k+1} = F_k P_k F_k^\top + G_k Q_k G_k^\top
$$

Inline: \\(\mathbf{J}^\top \mathbf{J}\\)

```cpp
Eigen::Matrix3d F = Eigen::Matrix3d::Identity();
P = F * P * F.transpose() + G * Q * G.transpose();
```

where `F` is the state transition matrix, `G` is the process noise input matrix,
and `Q` is the process noise covariance.
