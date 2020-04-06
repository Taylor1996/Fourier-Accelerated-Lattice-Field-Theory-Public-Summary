### This is the homepage for the public summary of my MPhys project, Fourier accelerated lattice field theory.

This public summary is aimed at those people who have completed Higher (or equivalent) level physics and like to read the science section of their favourite news website.

Our current understanding of how fundamental particles interaction in our universe envisions them as being little excitations in "quantum fields" which permeate space and time. The figure below shows an impression of a field with a single peak (excitation) localized in space. This peak can be thought of as a particle.  
![image](https://user-images.githubusercontent.com/26764889/78572038-dc624080-781e-11ea-9780-61a126b615f8.png)


<!--![image](https://user-images.githubusercontent.com/26764889/78559293-0f4f0900-780c-11ea-9d3a-51cda3c59ae2.png)-->

There are two main ways to study these fields theoretically in order to investigate properties of these particles:
1. Blackboard calculations involving Feynman diagrams.
2. Simulate the fields on a computer (lattice field theory).

My project looked at the 2nd of these approaches which is particularly useful in certain cases (such as in the theory of _quantum chromodynamics_ which describes the physics of quarks, the constituents of protons and neutrons).

In order to get an idea of how we carry out lattice field simulations on a computer, let us first look at simulating something that can be visualized a little easier. Thus, we turn our attention to the quantum mechanical harmonic oscillator. This is nothing much more than a system which will be quite familiar: a mass attached to a spring and allowed to oscillate back and forth. The quantum mechanics bit just means that the mass-spring system won't act quite as it is expected to in everyday life. 

Now, suppose you were to set up a frictionless table, and place on top of such a contraption consisting of a weight connected to a wall via a spring. You pull the mass away from its equilibrium point where it was stationary and let go. What you see is the motion below:

![classical_final](https://user-images.githubusercontent.com/26764889/78579416-cd808b80-7828-11ea-942f-05630130c676.gif)

If you pull the mass back the same distance and let go, you will observe the exact same motion every time.

Now, in the case of a quantum mechanical version of this harmonic oscillator, we find that the motion can be quite different. In fact, each time you watch the oscillator move in time, you will see it do something slightly different. This is because in quantum mechanics, a particle's position is a probabilistic thing - there is some porbability that at time t after you let go of the mass that it is at position A. However, there is also some probability that it is at position B. Only when you measure its position can you say for certain where the mass is.

As a consequence, there are infinitely many ways that the mass could have oscillated about on its spring (referred to as _paths_) in the quantum mechanical case. Albeit, some of these are more likely to be realized than others.

So how does all of this relate to our computer simulations? Well, it turns out that everything we may want to know about our quantum mass on a spring system is encoded in a mathematical object called the **path integral**. And without going into too much detail, this path integral is simply a sum of all those paths we talked about. Each of these paths are assigned a _weight_ - some probability that the path in question is that which the system follows. To simply add up all of these paths in a naive approach would be a lot of work (an infinite amount actually). Instead we use computational methods, called **Markov chain Monte Carlo** methods, to efficiently sum up these paths by choosing to look at paths with a greater probabilistic weight more often. This is termed importance sampling.







**Bold** and _Italic_ and `Code` text

[Link](url) and
 

