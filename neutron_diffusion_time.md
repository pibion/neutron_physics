
The Question
===========
Once neutrons reach the water in the Neutron Multiplicity Meter, the timescale for their capture is about 10 microseconds.  But how long does it take the neutron - born in the lead bricks beneath - to get to the water in the first place?


The Path
=======
If the motion of the neutron was similar to Brownian Motion (free travel punctuated by random changes in direction on a characteristic time scale), then we'd have a way forward.  Lucky for us, our neutron's movement is well described by Brownian motion: its energy changes very little because lead nuclei are so much heavier, and at these energies scattering is isotropic [citation needed].

So.  We can think of the neutron as flying freely between lead nuclei- but only for so long.  After some characteristic distance, the neutron will smack into a lead nucleus and emerge in a random direction to continue its journey.

The reason the neutron makes progress towards the water tank isn't because it was originally headed in that direction.  It's because the width of its position distribution increases, thus increasing its likelihood of being found further from its starting point.

If we assume that the width of the neutron's probability distribution obeys Poisson statistics, then $\sigma = \sqrt{N_{bounces}}$.

If we want to find the typical time for a neutron to wander some distance $L$ from its origin, we need to find the time such that
$$L = \sqrt{N_{bounces}} \lambda_{Pb},$$
where $\lambda_{Pb}$ is the neutron's average path length between collisions.

This leaves us with two questions to answer for a solution.
1. What's the relationship between lab time and how many times the neutron has bounced?
2. How can we express the neutron's characteristic path length in lead using known quantities?


Neutron Bounces 
==============
Over some time $t$, the neutron travels from lead nucleus to lead nucleus, changing direction with each collision.  

Now imagine the neutron's path between two of these nuclei.  This path length is drawn from a distribution about the average path length, and this average path length is what we call $\lambda_{Pb}$.  

For a neutron travelling at some (unchanging) velocity $v_n$, the average path length implies some average time: $t_{Pb} = \lambda_{Pb} / v_n$.  So the neutron's journey can be broken up into a series of pieces that have some characteristic distance, or alternatively, a series of pieces that take some characteristic time.

In time $t$, the number of bounces can be written $t \ t_{Pb}$, and
$$N_{bounces} = \frac{t}{t_{Pb}} = t \frac{v_n}{\lambda_{Pb}}.$$


What is $\lambda_{Pb}$?  What is $v_n$?
==================================
What is $v_n$?  I don't know.  You'll have to go look that up.

Taking some liberties, the characteristic path length $\lambda_n$ of a neutron in lead can be written
$$\lambda_{Pb} = \frac{1}{\rho_{Pb} \sigma_{Pb}(v_n)}.$$

The cross section, $\sigma_{Pb}$, should actually be marked as the _scattering_ cross section.  The total cross section can be written as the scattering plus the absorption cross section; we've been talking about the neutron "bouncing around" - that's the scattering cross section.  What we're assuming when we write the average path length this way is that the absorption cross section is much smaller than the scattering cross section.

Also note that the cross section isn't a constant!  It changes as the neutron's energy changes.

The cross section, like the expected neutron velocity, is something you'll need to look up.

And so.  A solution.
================
Ah, there we are. Imagine a stack of lead bricks in your laboratory. If a neutron is sprung free from its nucleus at a depth L from the surface of that lead, after what time $t_L$ can we expect it to emerge?  

Idealizing the neutron's motion and Poisson statistics allow us to reduce this question to: what is the time $t_L$ such that
$$ L = \sqrt{N_{bounces}} \lambda_{Pb}?$$

Substituting from above, 
$$ 
L = \sqrt{t_L \rho_{Pb} \sigma_{Pb}(v_n) v_n} \lambda_{Pb} 
\implies 
t_L = \frac{L^2 / \lambda_{Pb}^2}{\rho_{Pb} \sigma_{Pb}(v_n) v_n}.
$$

One can of course simplify this expression further, but I like this form for two reasons.
-- $L$ is "normalized" to units of $\lambda_{Pb}$.
-- The $\sigma v$ in the denominator offers a clue to the knowledgeable reader - at low energies, the cross section scales inversely with the velocity.  If your neutron is in that energy region, this term is ... constant.


Numbers for Lead
===============


Numbers for Neutrons
==================

> Written with [StackEdit](https://stackedit.io/).