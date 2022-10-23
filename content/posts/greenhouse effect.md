---
title: "Greenhouse Effect"
date: 2022-09-10
tags:
- notebook
- climate
---

*My notebook for the Coursera course: **Global Warming I: The Science and Modeling of Climate Change**, The University of Chicago.*

![[images/climate modeling/greenhouseeffect1.svg]]
The figure above depicts the previously described [[posts/naked planet climate model|first basic climate model with bare-rock surface]]. The incoming energy budget is represented by $\dfrac{L(1 - \alpha)}{4}$ in the figure, where L is the solar constant, α is the albedo of Earth, and number 4 represents the geometry of the system (we're considering the entire planet, so it's a sphere, keep this in mind because we'll deal with different problems that consider different conditions). This energy would be balanced by the energy that leaves the system, as indicated by $\epsilon \sigma T^4_{ground}$, where ε, σ and T are the emissivity of Earth, the Stefan-Boltzmann constant, and the Earth's ground temperature, respectively.

However, we discovered that the given model is rather cold in comparison to real-world values. This is due mostly to the presence of [[posts/greenhouse gases|greenhouse gases]] in the atmosphere, which absorb and emit radiation as well.

For the sake of simplicity, imagine all of the gases that absorb and emit as a pane of glass in the atmosphere.

![[images/climate modeling/greenhouseeffect2.svg]]
We will also make the following assumptions for this model:

- The pane of glass does not absorb sunlight.
- The glass absorbs infrared radiated by the earth.
- The glass pane itself emits infrared light in both directions, up and down, according to its own temperature T<sub>a</sub>.

We can then obtain some formulae for the various types of energy in the model:

- $\dfrac{L(1 - \alpha)}{4}$ is the incoming energy budget that the ground absorbs.
<br></br>
- $\epsilon \sigma T^4_{g}$ represents energy emitted by the ground.
<br></br>
- $\epsilon \sigma T^4_a$ represents energy absorbed and emitted by the pane of glass (assuming that the glass has good [[notes/blackbody|blackbody]] properties, ε ≈ 1)

Then we get the following table for the energy budgets that enter and exit the system:

|Energy budget|IN|OUT|
|------|:----:|:----:|
|Ground|$\dfrac{L(1 - \alpha)}{4}+\epsilon \sigma T^4_a$|$\epsilon \sigma T^4_g$|
|Atmosphere|$\epsilon \sigma T^4_g$|$2\epsilon \sigma T^4_a$|

To get the energy budget for the Earth system overall, we could add them up and obtain: $$\dfrac{L(1 - \alpha)}{4} = \epsilon \sigma T^4_a$$

However, there is a simpler, much less complicated solution: create a general budget that depicts the whole system. We may draw a line above the atmosphere representing the border to space (as depicted in the figure). And the results would be the same as what we obtained previously.

|Energy budget|IN|OUT|
|------|:----:|:----:|
|Ground|$\dfrac{L(1 - \alpha)}{4}$|$\epsilon \sigma T^4_a$|

