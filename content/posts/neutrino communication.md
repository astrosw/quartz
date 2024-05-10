---
title: Neutrino-based Communication
date: 2022-08-05
tags:
  - particle
  - physics
  - discussions
---

(still writing...)

***DISCLAIMER:*** *Particle Physics is not my area of study. Please let me know if you notice any mistakes or omissions.*

In this post, I'll discuss the possibility of using [[notes/neutrinos|neutrinos]] for communication between New York and Tokyo and answer the questions: What can we gain with neutrino-based communication in comparison to the conventional communications? What's the most challenging for developing this kind of communication?

Of course in order to discuss all that, we need to grasp the basic concepts. The first question is undoubtedly:

## What are neutrinos?

Basically they are elementary particles that have neutral charge and very VERY small mass (thought to be massless for a long time). They are [[notes/fermions|fermions]] that interact only via the [[notes/weak interactions|weak interactions]] and [[notes/gravity|gravity]].

*Well, I do realize the above explanation is still a little vague for those who are unfamiliar with particle physics (like me). Like okay, they're fermions, but what are fermions? What exactly are elementary particles? Where do they exist in atoms, and how do they connect with other particles that we are more familiar with, such as electrons, protons, and neutrons? And so i decided to set up this site to utiliize the power of bidirectional links. You can move to the individual notes of each concept by clicking on the internal links, or you can look at how these are connected in the interactive graph at the bottom.*

## Why neutrinos for communication?

Neutrinos can essentially travel through anything and everything. They can propagate through vast cosmic distances without significant attenuation or deflection. This is because they have relatively weak interactions and can't be caught by other particles. This capability makes neutrino a potential messenger for future global point-to-point communication, communication with submarines, interstellar communication or even planetary exploration! Isn't that exciting?

*Neutrinos are often described as tiny particles or as having weak interactions. These phrases might a little bit confusing, though. "Probability of interaction is small" or "neutrino interaction is rare" are more suitable expressions to explain their penetrating characteristic.*

*The concept of cross section would be helpful in comprehending this rarity. Cross section (σ(cm<sup>2</sup>) is the size of the target particle from a view point of interaction. For example, if 1 GeV protons interact with the target nuclei, the interaction is a hadron interaction with a cross section of σ ~ 3 x 10<sup>-26</sup> cm<sup>2</sup>. On the other hand, if 1 GeV neutrinos encounter the target nuclei, the interaction is weak, with a cross section of about σ ~ 1 x 10<sup>-38</sup> cm<sup>2</sup>. It is smaller than that of hadron interaction by a factor of 3 x 10<sup>12</sup>.*


## Operation and Challenges

### A past experiment

Neutrino-based communication is thus an intriguing concept, but is it realistic?

Weak interactions seem to provide neutrinos the benefit of penetrating matter, but this same property also suggests that very powerful beams and HUGE massive detectors would be required. These are regarded as the two major obstacles to implementing this kind of communication.

An [experiment](https://arxiv.org/abs/1203.2847) had been conducted in 2012 using the NuMI beam line and the MINERvA detector to perform low-rate communications over a distance of about 1 km. 

### Path length and matter effect

In our scenario, however, we wish to send information from New York to Tokyo across the earth at a distance of about 9600 km. There have been concerns about whether the huge traveling distance might weaken the beam because it is very large in comparison to the experiment.

There are several ways to answer this.

You can use the following formula to calculate the number of particles left (N) after traveling a distance (x):
$$
N = N_0e^{-\sigma \rho x}
$$

where N<sub>0</sub> is the initial number of particles, σ is the interaction cross section and ρ is the density of matter which the particle pass through.

So when the particle is a neutrino, we all know that the cross section is very small, about 10<sup>-38</sup> cm<sup>2</sup>/GeV. For the density, we can take the standard density of rock, which is 2.65 g/cm<sup>3</sup>, and x would be 9600km. So the reduction should be really really small, even if the path length is very long and the neutrino energy is very high.

We can use another method to tackle this problem. Let's have a look at the plot below

![[images/particle physics/maxmeier.jpg]]

This is a plot that shows the neutrino attenuation during propagation through the Earth. The x-axis is the zenith angle. The left y-axis shows the survival probability of a neutrino, and the right y-axis shows the slant depth in meters of water equivalent that the neutrino at that zenith angle would be passing through. So for our problem, we have 9600 km, if we take the standard density of rock of 2.65 g/cm<sup>3</sup>, then 9600 km of rock would correspond to approximately 26000 km of water equivalent. So according to this plot, going from New York to Tokyo would correspond to a zenith angle of 110<sup>o</sup>. For a 120 GeV beam, for example, we should expect almost no neutrino attenuation. Of course this is just rough estimation.

We can also calculate the neutrino survival probability by ourselves using this formula:
$$
P_{surv} = e^{-N_A\sigma_{E_{nu}}X}
$$

where N<sub>A</sub> is the Avogadro constant, σ<sub>E<sub>nu</sub></sub> is the total neutrino cross section at energy E<sub>nu</sub>, and X is the slant depth in meters water equivalent. To calculate the slant depth you can use a density model of the Earth like [this](https://de.wikipedia.org/wiki/PREM).

Regarding the neutrino oscillations, at ~100 GeV energies neutrino oscillations can change the flavour of our neutrino beam. But most likely our neutrino detector will be able to detect all neutrino flavours. So if the idea of communication is similar to the past experiment using NuMI beam line and MINERvA detector (encoding communication bits by the neutrino beam being either on or off), I think the flavour composition of the neutrino beam should not be relevant.

There is another approach to the flavour change problem. When a mu-neutrino oscillates to a tau-neutrino and the energy is less than tau production threshold, charged current (CC) interactions never happen. In this case, the neutrino oscillation affects the detection. However the energy that was used (and will be used) is higher enough than the tau production threshold. (I think the interaction cross sections $\nu_e$, $\nu_{\mu}$ and $\nu_{\tau}$ can be assumed to be the same; neutral current (NC) cross sections are always the same for $\nu_e$, $\nu_{\mu}$ and $\nu_{\tau}$).



<!---
### Beam intensity

numi

### Detector

minerva

## Conclusion
-->
