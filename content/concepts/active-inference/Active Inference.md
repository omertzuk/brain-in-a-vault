---
title: Active Inference
aliases:
  - AIF
  - Active Inference Framework
tags:
  - active-inference
  - cognitive-science
  - bayesian-brain
  - predictive-processing
  - information-theory
status: seed
---

# Active Inference

**Active Inference** is a framework for understanding how an [[Agent]] perceives, learns, and acts in a changing [[Environment]].

The basic idea is that the brain does not passively receive the world “as it is.” Instead, it behaves like a [[Hypothesis testing brain]]: it continuously generates predictions about the causes of its sensory input, checks those predictions against incoming data, and updates its internal model when prediction and reality do not match.

In this sense, Active Inference belongs to the broader family of ideas known as the [[Bayesian brain hypothesis]] and [[Predictive processing]].

## Core intuition

The agent is always separated from the world by a [[Statistical boundary]], often described in Active Inference as a [[Markov blanket]].

Because of this boundary, the agent never has direct access to the true structure of the world. It only receives [[Sensory observations]].

This creates the central problem:

> Given only sensory data, how can an agent infer what is happening in the world and decide what to do next?

This is the [[Inverse problem]].

## The Box Scenario

The [[Box scenario]] is a useful thought experiment.

Imagine that you are trapped inside a box. You cannot see the outside world directly. You only receive information from noisy sensors. Your task is to survive by learning which sensory signals predict danger, safety, resources, or opportunities for action.

This scenario illustrates the situation of any biological organism:

- it does not directly perceive the world;
- it receives partial and noisy [[Sensory observations]];
- it must infer hidden causes;
- it must distinguish [[Signal]] from [[Noise]];
- it must act quickly enough to remain viable.

## Generative process and generative model

Active Inference distinguishes between two important ideas:

### [[Generative process]]

The [[Generative process]] is the real-world process that produces sensory data.

For example, in the [[Box scenario]], something outside the box produces signals that reach the sensors. The true causes may be physical objects, events, patterns, or dangers in the environment.

### [[Generative model]]

The [[Generative model]] is the agent’s internal model of how sensory data are generated.

It is not the world itself. It is the agent’s best internal representation of how the world might work.

The agent uses this model to infer [[Hidden states]] of the world from sensory input.

## Hidden states

[[Hidden states]] are the causes of sensory observations that the agent cannot access directly.

For example:

- a predator nearby;
- food behind a tree;
- a dangerous storm approaching;
- another person’s emotional state;
- the true state of the environment outside the [[Box scenario]].

The agent must infer hidden states from the available evidence.

## Structure, information, and prediction

A central assumption of Active Inference is that the world has [[Structure]], [[Order]], [[Regularities]], and often [[Hierarchies]].

If the world were completely random, there would be no stable pattern to learn. The agent could not predict anything, because every sensory observation would be unrelated to previous observations.

This is where [[Information Theory]] becomes important.

In [[Information Theory]], structure is closely related to [[Predictability]]. A signal contains usable information when it has patterns that can be learned and used to reduce [[Uncertainty]].

So the task of the agent is not merely to receive data. It must discover the hidden structure behind the data.

In other words:

> The agent receives sensory signals and tries to reconstruct the process that generated them.

This is why perception is a form of [[Reconstruction]]. The agent uses its [[Generative model]] to reconstruct the hidden [[Generative process]] behind its sensory observations.

## Compression and generative models

A good [[Generative model]] is not a perfect copy of the world. It is more like a [[Compressed representation]] of the world’s causal structure.

This means that the agent does not need to store every sensory detail. Instead, it needs to capture the deeper patterns that explain many observations.

For example, instead of remembering every single visual angle of a tree, the brain learns a compact model of “tree-ness”: trunk, branches, leaves, seasonal changes, typical locations, and possible actions.

This connects Active Inference with several ideas from [[Information Theory]]:

- [[Entropy]] — how uncertain or unpredictable a signal is;
- [[Redundancy]] — repeated structure in the signal;
- [[Signal-to-noise ratio]] — how much useful signal is mixed with irrelevant variation;
- [[Compression]] — representing a process efficiently;
- [[Mutual information]] — how much knowing one variable tells us about another;
- [[Uncertainty reduction]] — the process of making future states more predictable.

## The inverse problem

The [[Inverse problem]] is difficult because the agent receives only sensory effects, not the hidden causes themselves.

The agent must move backward:

> From sensory data → to possible hidden causes.

But this is hard because the same sensory signal can be produced by many different causes.

For example, a loud sound could mean:

- thunder;
- a falling object;
- an animal nearby;
- a human action;
- a machine malfunction;
- an echo.

The agent must infer which hidden state most likely generated the observation.

## Why the inverse problem is hard

Several factors make [[The Inverse Problem]] difficult.

### 1. Nonbijective mappings

If every environmental state produced one unique sensory signal, inference would be easy.

This would be a [[Bijective mapping]].

But real perception is usually [[Nonbijective]].

Sometimes many hidden causes can produce the same sensory signal. This is a [[Many-to-one mapping]].

Sometimes one hidden cause can produce many different sensory signals. This is a [[One-to-many mapping]].

This makes perception ambiguous.

### 2. Mixed signals

The environment is dynamic. Signals do not arrive separately and cleanly.

They often mix together.

For example, when listening in a crowded room, your ears receive a mixture of voices, echoes, background noise, music, and bodily sounds.

The brain must perform something like [[Signal unmixing]] to infer which hidden causes produced the sensory data.

### 3. Correlation is not causation

The agent must distinguish [[Correlation]] from [[Causation]].

Two signals may occur together without one causing the other.

For example, a sound and a shadow may appear at the same time, but both may be caused by a third hidden factor.

This is the problem of [[Confounding variables]].

### 4. Noise and uncertainty

The agent samples sensory signals in a noisy world.

This means that perception is always probabilistic. The sensory data may be corrupted by irrelevant variation, measurement error, or limitations of the nervous system.

The agent must separate [[Signal]] from [[Noise]].

This is essential for adaptive behavior, because the organism must know what information matters for action.

### 5. Future states cannot be fully verified in advance

The agent often makes predictions about future states.

But a future prediction can only be fully tested when the future actually occurs.

This means the agent must act under [[Uncertainty]].

It cannot wait for perfect knowledge.

### 6. Exact inference is often impossible

The [[Inverse problem]] may be too complex to solve exactly.

A biological organism does not have unlimited time or computation. It must act before it starves, freezes, gets injured, or is eaten.

Therefore, the agent often needs an [[Approximate inference]] strategy.

It sacrifices perfect accuracy for a solution that is good enough to survive.

This connects Active Inference with [[Heuristics]], [[Bounded rationality]], and [[Adaptive behavior]].

## Bayesian inference

The mathematical foundation of this process is [[Bayesian inference]].

In simplified form, the agent combines:

- a [[Prior]] — what it already expects;
- a [[Likelihood]] — how probable the sensory data are under a given hypothesis;
- [[Model evidence]] — how well the model explains possible observations;
- a [[Posterior]] — the updated belief after receiving evidence.

This means that perception is not just “receiving data.” It is an active process of inference.

## Acting as inference

In Active Inference, action is also part of the same process.

The agent does not only update beliefs to fit the world. It can also act on the world so that sensory input better matches its predictions.

For example, if I believe there is danger nearby, I may move, look around, or escape. These actions generate new sensory data that help confirm or revise my model.

So Active Inference links:

[[Perception]] → [[Inference]] → [[Action]] → [[Learning]]

## Why “active”?

The framework is called **Active Inference** because the agent does not merely infer passively.

It actively samples the world.

It moves, explores, tests hypotheses, and changes its relation to the environment in order to reduce uncertainty and maintain itself.

## Why this matters

Active Inference gives us a unified way to think about:

- [[Perception]]
- [[Action]]
- [[Learning]]
- [[Embodied cognition]]
- [[Predictive processing]]
- [[Bayesian inference]]
- [[Information Theory]]
- [[Adaptive behavior]]
- [[Artificial agents]]
- [[Biological agents]]

It is especially useful because it frames the brain as a living, embodied system that must continuously model and act within a dynamic world.

## Key distinction

A simple way to remember the framework:

> The world generates sensory data through the [[Generative process]].  
> The agent explains those data using its [[Generative model]].  
> The better the model captures the structure of the world, the better the agent can predict and act.

## Related notes to create next

- [[Hypothesis testing brain]]
- [[Box scenario]]
- [[Bayesian brain hypothesis]]
- [[Predictive processing]]
- [[Generative model]]
- [[Generative process]]
- [[Hidden states]]
- [[Sensory observations]]
- [[Bayesian inference]]
- [[Bayes theorem]]
- [[Prior]]
- [[Likelihood]]
- [[Posterior]]
- [[Model evidence]]
- [[Inverse problem]]
- [[Markov blanket]]
- [[Agent]]
- [[Environment]]
- [[Prediction error]]
- [[Embodied cognition]]
- [[Information Theory]]
- [[Entropy]]
- [[Predictability]]
- [[Uncertainty]]
- [[Signal]]
- [[Noise]]
- [[Signal-to-noise ratio]]
- [[Compression]]
- [[Compressed representation]]
- [[Mutual information]]
- [[Redundancy]]
- [[Correlation]]
- [[Causation]]
- [[Confounding variables]]
- [[Approximate inference]]
- [[Heuristics]]
- [[Bounded rationality]]