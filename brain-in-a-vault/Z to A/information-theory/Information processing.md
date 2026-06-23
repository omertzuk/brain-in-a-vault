---
aliases:
  - Computation
title: Information Processing
---
- Let's start with propositions that can be True or False:
	- $X=$ it's sunny
	- $Y=$ it's rainy
	- $X \, AND \, Y$ (usually False, but could be True in principle)
- Boole developed notations:
	- $X \, AND \, Y \equiv X \land Y$,  $X \, OR \, Y \equiv X \lor Y$
- Boole showed that any possible logical proposition can be written in those terms.
- Any set of digital logic operation can be broken down into $\land$, $\lor$, $\lnot$ , and copy operations.
- So we can use information to label things (names, barcodes)
- So what is the probability that it is rainy AND it is sunny? 
- The joint probability of $X$ and $Y$ - $P(X \land Y)\equiv P(XY)$
- The [[Marginal probability]] of $X$ is $P(X)=P(XY)+P(X \tilde Y)$
- So this leads us to the [[Mutual Information]] 