---
title: Mutual Information
---
- So if we have $X_i, Y_j$ - set of events, and $P(X_i, Y_i)$, we can talk about the joint information, the information that is inherent in the joint event: $$I(XY)=-\sum_{il} p(x_iy_i)\log_2p(x_iy_i) $$
- So the joint information for $x$ would be here $I(x)=\sum_i p(x_i)\log_2p(x_i)$
- So the *mutual information* (*$:$*) would be: $$I(X:Y)=I(X)+I(Y)-I(XY)\geq0 $$
- If $X$ and $Y$ are completely uncorrelated, the mutual information would be zero.
- So mutual information is measures the amount of information that $X$ can tell us about $Y$, and it is symmetric. So another way to think about it is the amount of information $X$ and $Y$ hold in common.
- The mutual information allows us to calculate [[Communication Capacity]].