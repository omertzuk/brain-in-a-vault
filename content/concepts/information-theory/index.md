---
title: Information Theory
permalink: information-theory
---
- What is the relationship between [[Information]] and [[Probability]]? To think on probability we can start with [[Flipping a coin]]:
	- So if we have a fair coin we have $p(H)=p(T)=\frac{1}{2}$
	- But we can think about it from a frequentist perspective that if we toss the coin many $N$ times we will converge to Tail and Head appearing $N/2$ times
	- So the number of ways of choosing $m_H$ "spots" out of $m$ possible spots - so we mark ${m \choose m_H} = \frac{m!}{m_H!\left(m-m_H\right)!}= \frac{m!}{m_H!m_T!}$
	- So the frequency of heads, what we observe, is $q(H)\equiv \frac{\#heads}{m}$
	- So the [[Fundamental Formula of Information Theory]] says that $$S = -q(H)\log_2q(H)-q(T)\log_2q(T)$$
	- So suppose we observe $q(H)=1/2=q(T)$, we will get that $S=-(-1)=1 \, bit$ 
	- This formula says that if I have a coin and the frequency of head and tail is one half, than the amount of information that is given in *one flip* is $1\,bit$
- To be continue...